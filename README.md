# 🖥️ Página de Vendas — Imersão GOF | Leo Soares · LTX Group

Landing page de vendas de alta conversão para a **Imersão GOF (Gestor de Operações Financeiras)**, evento presencial de 1 dia com Leo Soares, realizado pela LTX Group em Eusébio, CE.

---

## 📋 Sobre o Projeto

Página de vendas single-page desenvolvida com HTML, CSS e JavaScript puro — sem frameworks, sem dependências de build. O layout segue uma estética financeira sóbria e premium, com fundo escuro, tipografia serifada e acentos em verde-teal, transmitindo credibilidade e urgência ao visitante.

**Evento:** Imersão GOF — 1 dia presencial com Leo Soares  
**Data:** 02 de maio (sábado), das 9h às 17h  
**Local:** Sede da LTX Group — Cidade Alpha, Eusébio, CE  
**Vagas:** Limitadas a 30 participantes  
**Preço:** R$ 497 com garantia incondicional de 7 dias

---

## 🗂️ Estrutura da Página

A página é composta pelas seguintes seções, de cima para baixo:

| Seção | Descrição |
|---|---|
| **Urgency Bar** | Barra fixa no topo com contador regressivo de prazo |
| **Ticker** | Faixa animada com tickers de ativos financeiros (estética de mercado) |
| **Hero** | Headline principal, promessa central e CTA acima da dobra |
| **Stats Strip** | 4 números sociais de prova (alunos, retorno, anos, gestão) |
| **Problem Section** | Lista de dores do público-alvo |
| **Candle Strip** | Decoração visual com velas de candlestick e citação de destaque |
| **What Section** | O que é a imersão + grade com os 6 módulos/partes do conteúdo |
| **Gains Section** | Transformações esperadas após o evento + cards de mercado |
| **Who For** | Perfil do participante ideal (empresários, profissionais liberais, executivos) |
| **Mentor** | Bio e credenciais de Leo Soares |
| **Event Info** | Data, horário, endereço e contagem de vagas |
| **Guarantee** | Garantia incondicional de 7 dias |
| **Inscription** | Seção de preço e botão de compra principal |
| **FAQ** | 7 perguntas frequentes com acordeão interativo |
| **Final CTA** | Último chamado antes do rodapé |
| **Footer** | Créditos, aviso legal e links de política |
| **Sticky Mobile** | Botão fixo no rodapé para dispositivos móveis |

---

## 🛠️ Tecnologias Utilizadas

- **HTML5** — marcação semântica, sem frameworks
- **CSS3** — custom properties (variáveis), grid, flexbox, animações e responsividade
- **JavaScript (vanilla)** — contador regressivo com persistência via `localStorage`, acordeão do FAQ
- **Google Fonts** — `Playfair Display`, `DM Sans`, `DM Mono`

---

## 🎨 Design System

```
Cores principais:
  --black:  #080A0D   (fundo base)
  --teal:   #00C8A0   (cor de destaque / CTA)
  --white:  #F0EDE8   (texto principal)
  --muted:  #8A9BAE   (texto secundário)
  --red:    #E05555   (elementos negativos / dores)

Tipografia:
  Títulos:  Playfair Display (serif, elegante)
  Corpo:    DM Sans (sans-serif, legível)
  Mono:     DM Mono (tickers, labels técnicos)
```

---

## ⚙️ Funcionalidades Interativas

- **Contador regressivo** com persistência em `localStorage` — o timer não reinicia ao recarregar a página
- **Ticker animado** com loop contínuo via CSS `@keyframes`
- **FAQ acordeão** — abre/fecha perguntas via JavaScript
- **Botão sticky mobile** — aparece no rodapé em telas pequenas
- **Scroll suave** entre seções via `scroll-behavior: smooth`
- **Velas (candlestick)** geradas dinamicamente via JavaScript com alturas e cores aleatórias

---

## 📁 Arquivos

```
/
└── pagina-de-vendas-imersao-gof.html   # Arquivo único — toda a página
```

> A página foi desenvolvida como arquivo único (HTML + CSS + JS inline), facilitando o deploy em qualquer hospedagem estática.

---

## 🚀 Como Usar

### 1. Clonar o repositório

```bash
git clone https://github.com/seu-usuario/pagina-de-vendas-imersao-gof.git
cd pagina-de-vendas-imersao-gof
```

### 2. Dependências

> **Nenhuma.** O projeto é um arquivo HTML único com CSS e JavaScript inline.  
> Não há `package.json`, `node_modules` nem etapa de build — basta abrir o arquivo no navegador.

### 3. Rodar localmente

```bash
# Opção A — abrir direto no navegador (mais simples)
open pagina-de-vendas-imersao-gof.html

# Opção B — servir via servidor local (evita restrições de localStorage em alguns navegadores)
npx serve .
# ou
python3 -m http.server 8080
```

Acesse `http://localhost:8080` no navegador.

### 4. Deploy

Basta fazer upload do arquivo para qualquer hospedagem estática:

- **Vercel:** arraste o arquivo no dashboard ou use `vercel deploy`
- **Netlify:** arraste o arquivo em [app.netlify.com/drop](https://app.netlify.com/drop)
- **GitHub Pages:** suba o arquivo como `index.html` na branch `gh-pages`

> **Atenção:** antes de ir ao ar, atualize os links dos botões de compra (`href="#"`) com a URL real do checkout, e os links de Termos de Uso e Política de Privacidade no rodapé.

---

## ✏️ Personalizações Comuns

| O que mudar | Onde encontrar no código |
|---|---|
| Data e horário do evento | Seção `#event-info` e FAQ |
| Preço | Seção `#inscricao` → `.price-main` |
| Link de compra | Botões `btn-primary` com `href="#"` |
| Prazo do contador | Variável `target` no `<script>` no final do `<body>` |
| Tickers financeiros | Elementos `.ticker-item` na seção `.ticker-bar` |
| Número de vagas | Seção de inscrição, event card e FAQ |

---

## 📄 Licença

Projeto proprietário — desenvolvido para uso exclusivo da **LTX Group / Leo Soares**.  
© 2026 LTX Group · Todos os direitos reservados.
