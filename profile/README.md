

<h1 align="center">💸 Poupa Pobre</h1>

<p align="center">
  <strong>Sistema de finanças pessoais — "a planilha evoluída".</strong><br>
  Controle de receitas, gastos, cartões, dívidas, metas e patrimônio com o nível de
  detalhe e customização que os apps comuns não entregam. Cada pessoa é dona dos seus
  dados e compartilha lançamentos específicos, item a item, com quem quiser.
</p>

<p align="center">
  <img src="profile/assets/tela-inicial.jpeg" alt="Tela inicial do Poupa Pobre" width="280">
</p>

---

## 📱 Sobre o projeto

O **Poupa Pobre** organiza a vida financeira em torno do **mês**: você abre o app e vê
na hora o que já saiu e o que ainda vem. São 8 módulos — Receitas, Gastos do dia a dia
(com **scanner de cupom fiscal**), Gastos fixos, Cartão de crédito, Dívidas, Metas,
Investimentos e Patrimônio líquido.

Entrega **mobile-first** (app React Native), com a API REST e a documentação do produto
em repositórios separados:

| Repositório | Descrição |
|---|---|
| [**mobile**](https://github.com/poupa-pobre/mobile) | App React Native + Expo (Fase 1) |
| [**backend**](https://github.com/poupa-pobre/backend) | API Django REST + PostgreSQL |
| [**documentacao**](https://github.com/poupa-pobre/documentacao) | Visão, requisitos, modelo de dados e fluxo de telas |

## 🛠️ Tecnologias utilizadas

**Mobile**
![React Native](https://img.shields.io/badge/React%20Native-61DAFB?logo=react&logoColor=black)
![Expo](https://img.shields.io/badge/Expo-000020?logo=expo&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![NativeWind](https://img.shields.io/badge/NativeWind%20(Tailwind)-06B6D4?logo=tailwindcss&logoColor=white)

**Backend**
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?logo=django&logoColor=white)
![DRF](https://img.shields.io/badge/Django%20REST-A30000?logo=django&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?logo=jsonwebtokens&logoColor=white)

**Infra**
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Oracle Cloud](https://img.shields.io/badge/Oracle%20Cloud-F80000?logo=oracle&logoColor=white)

## 👥 Integrantes

<!-- Substitua pelos nomes reais da equipe -->
- [@JuscelinoJunior](https://github.com/JuscelinoJuniorFC)
- [@lucasRudyson](https://github.com/lucasRudyson)


## 🚀 Instruções básicas de execução

São dois projetos: o **backend** (API) e o **mobile** (app). Suba o backend primeiro.

### 1. Backend (Django + PostgreSQL via Docker)

```bash
git clone https://github.com/poupa-pobre/backend.git
cd backend
cp .env.example .env          # troque DJANGO_SECRET_KEY por uma string longa e aleatória
docker compose up --build     # API em http://localhost:8000
```

### 2. Mobile (React Native + Expo)

```bash
git clone https://github.com/poupa-pobre/mobile.git
cd mobile
npm install
cp .env.example .env          # ajuste EXPO_PUBLIC_API_URL (ex.: http://10.0.2.2:8000 no emulador Android)
npm start                     # escaneie o QR no app Expo Go
```

> Passo a passo detalhado (pré-requisitos, execução sem Docker e scanner de cupom)
> nos arquivos `SETUP.md` de cada repositório.

---

<p align="center"><sub>Projeto acadêmico de finanças pessoais · Poupa Pobre</sub></p>
