# Digital Store - E-commerce

Uma aplicação de e-commerce moderna desenvolvida com React, TypeScript e Tailwind CSS. Parte do projeto avaliativo **PROJETO GERAÇÃO TECH** do Instituto Euvaldo Lodi (IEL-CE) em parceria com o Governo do Estado do Ceará.

## 🎯 Sobre o Projeto

Digital Store é uma plataforma de e-commerce especializada na venda de sneakers e produtos relacionados. O projeto demonstra boas práticas de desenvolvimento frontend, incluindo gerenciamento de estado, roteamento, componentes reutilizáveis e design responsivo.

## ✨ Funcionalidades

- **Catálogo de Produtos**: Visualização de produtos com imagens, preços e descontos
- **Busca e Filtros**: Busca por nome/tipo de produto e filtros por marca, categoria, gênero e sessão
- **Detalhes do Produto**: Página dedicada com galeria de imagens, descrição completa e opções de tamanho
- **Produtos Relacionados**: Sugestões baseadas na marca do produto visualizado
- **Ordenação**: Ordenar por preço (menor/maior) e relevância
- **Design Responsivo**: Interface otimizada para desktop, tablet e mobile
- **Carrosel de Imagens**: Galeria interativa com Swiper.js
- **Animações Suaves**: Efeitos com Framer Motion

## 🛠️ Tecnologias Utilizadas

### Frontend
- **React 18.3** - Biblioteca UI
- **TypeScript 5.5** - Tipagem estática
- **React Router DOM 6.24** - Roteamento
- **Tailwind CSS 3.4** - Estilização
- **Framer Motion 11.3** - Animações
- **React Icons 5.2** - Ícones
- **Swiper 11.1** - Carrosséis
- **React Select 5.8** - Componentes Select
- **Axios 1.7** - Requisições HTTP

### Build & Dev Tools
- **Vite 5.3** - Build tool
- **ESLint 8.57** - Linting
- **Prettier 3.3** - Formatação
- **PostCSS 8.4** - Processador CSS

## 📋 Pré-requisitos

- Node.js 18+ 
- npm ou yarn
- Backend API rodando em `http://localhost:3333`

## 🚀 Como Executar

### Instalação

```bash
# Clone o repositório
git clone https://github.com/digitalcollegebr/projeto-digital-store.git

# Acesse o diretório
cd e-commerce_frontend

# Instale as dependências
npm install
```

### Desenvolvimento

```bash
# Inicie o servidor de desenvolvimento
npm run dev

# A aplicação estará disponível em http://localhost:3000
```

### Build para Produção

```bash
# Gere o build otimizado
npm run build

# Visualize o build localmente
npm run preview
```

### Linting

```bash
# Verifique problemas de linting
npm run lint
```

## 📁 Estrutura do Projeto

```
src/
├── assets/              # Imagens e ícones
├── components/          # Componentes reutilizáveis
│   ├── Banner/
│   ├── Button/
│   ├── BuyBox/
│   ├── CategoryCard/
│   ├── Discount/
│   ├── FeaturedCard/
│   ├── FilterCard/
│   ├── Footer/
│   ├── Gallery/
│   ├── Header/
│   ├── Layout/
│   ├── Logo/
│   ├── NotFound/
│   ├── OrderCard/
│   ├── ProductCard/
│   ├── ProductDetails/
│   ├── ProductListing/
│   ├── ProductOptions/
│   └── Section/
├── context/             # Context API para estado global
│   └── useProductContext.tsx
├── enum/                # Enumerações
│   └── index.tsx
├── interface/           # Tipos TypeScript
│   └── index.tsx
├── mock/                # Dados mockados
│   └── index.tsx
├── pages/               # Páginas da aplicação
│   ├── HomePage/
│   │   ├── HeroSection/
│   │   ├── CollectionSection/
│   │   ├── HotSection/
│   │   └── SpecialSection/
│   ├── ProductListingPage/
│   └── ProductViewPage/
├── routes/              # Configuração de rotas
│   └── index.tsx
├── service/             # Serviços (API)
│   └── index.tsx
├── styles/              # Estilos globais
│   └── global.css
├── utils/               # Funções utilitárias
│   ├── Price/
│   │   ├── FormatPrice/
│   │   └── DiscountPrice/
│   └── Timeout/
├── App.tsx
├── main.tsx
└── vite-env.d.ts
```

## 🎨 Configuração de Estilos

O projeto utiliza **Tailwind CSS** com cores personalizadas:

### Paleta de Cores
- **Primária**: `#C92071` (rosa)
- **Secundária**: `#B5B6F2` (roxo)
- **Terciária**: `#991956` (rosa escuro)
- **Cinzas**: `#1F1F1F` até `#F5F5F5`

### Fonte
- **Principal**: Inter (Google Fonts)

## 🔀 Rotas Disponíveis

| Rota | Descrição |
|------|-----------|
| `/` | Página inicial com seções de destaque |
| `/produtos` | Catálogo com filtros e busca |
| `/produto/:slug` | Detalhes do produto individual |
| `*` | Página 404 |

## 📦 Componentes Principais

- **Layout** - Wrapper com Header, Footer e ProductProvider
- **HomePage** - Seção inicial com collections e destaques
- **ProductListingPage** - Lista de produtos com filtros avançados
- **ProductViewPage** - Detalhes completos do produto
- **ProductCard** - Card reutilizável de produto
- **FilterCard** - Painel de filtros
- **Gallery** - Galeria de imagens interativa

## 🔌 Integração com API

A aplicação se comunica com uma API backend via Axios:

**Endpoints esperados:**
- `GET /products` - Lista todos os produtos
- `GET /product/:slug` - Detalhes de um produto

**Base URL:** `http://localhost:3333/`

## 🎯 Gerenciamento de Estado

Utiliza **Context API** com `useProductsContext` para compartilhar dados globais como lista de produtos, filtros e ordenação.

## 📱 Responsividade

Suporte completo para desktop, tablet e mobile com breakpoints do Tailwind CSS.

## 📜 Licença

Este projeto está licenciado sob a **Licença MIT** - veja o arquivo `LICENSE` para mais detalhes.

## 👥 Autores

Lucas Cavalcante dos Santos
[Github](https://github.com/cavalcanteprofissional)
[Linkedin](https://www.linkedin.com/in/cavalcante-lucas/)

## 🙏 Agradecimentos

- Instituto Euvaldo Lodi (IEL-CE) pela oportunidade e orientação
- Governo do Estado do Ceará pelo apoio ao programa
- Digital College Brasil pela estrutura do projeto
- Comunidade open source pelas bibliotecas e ferramentas utilizadas

## 🔗 Recursos Oficiais

- [Repositório Oficial](https://github.com/digitalcollegebr/projeto-digital-store)
- [E-commerce Digital Store](https://digital-store-web.vercel.app/)

---

**Versão**: 1.1.6 | **Último atualizado**: Dezembro 2025