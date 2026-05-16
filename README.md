# Fusion Lab — Arquitetura · Tech · Vida

Um espaço de fusão entre arquitetura, tecnologia, empreendedorismo e reflexões sobre a vida.

## 🚀 O que é

**Fusion Lab** é um blog pessoal que discute:
- 🏗️ **Arquitetura bioclimática** e design sustentável
- 💻 **Tecnologia aplicada** a arquitetura e design
- 🚀 **Empreendedorismo** e carreira em arquitetura
- 🧠 **Reflexões pessoais** sobre construir algo que valha a pena

Posts longos toda semana + briefs 3× por semana, sempre com opinião, nunca neutro.

---

## 📋 Como funciona

A página é 100% **HTML, CSS e JavaScript** — sem dependências externas:

- ✅ **Responsivo** — funciona em desktop, tablet e mobile
- 🌐 **3 idiomas** — Português, Inglês, Espanhol
- 📱 **PWA ready** — preparado para Progressive Web App
- ⚡ **Rápido** — todo CSS inline, sem frameworks
- ♿ **Acessível** — semântica HTML5 correta, suporte a screen readers

---

## 🛠️ Estrutura

```
fusion-lab/
├── index.html          # Página principal (HTML + CSS + JS integrados)
├── data.json           # Base de dados dos posts, notícias e ferramentas
├── config.json         # Configurações (API, analytics, etc)
├── api/
│   ├── subscribe.js    # Endpoint para newsletter
│   └── analytics.js    # Rastreamento personalizado
└── README.md           # Este arquivo
```

---

## 🚀 Como iniciar

### Opção 1: Localmente (sem servidor)
```bash
# Apenas abra o index.html no navegador
open index.html
```

### Opção 2: Com servidor local
```bash
# Python 3
python -m http.server 8000

# Node.js
npx http-server
```

Depois acesse: `http://localhost:8000`

### Opção 3: GitHub Pages (Deploy gratuito)
1. Vá para **Settings** → **Pages**
2. Source: `main` branch
3. Save

Seu site estará em: `https://ggabrielmorais-afk.github.io/fusion-lab`

---

## 📝 Adicionar posts

Edite `data.json` e adicione um novo objeto no array `posts`:

```json
{
  "id": 5,
  "slug": "seu-slug-aqui",
  "category": "Arquitetura",
  "title_pt": "Seu título em português",
  "title_en": "Your title in English",
  "title_es": "Su título en español",
  "excerpt_pt": "Resumo breve",
  "date": "2026-05-10",
  "readTime": 8,
  "views": 0,
  "likes": 0
}
```

---

## 📰 Adicionar notícias

Edite `data.json` e adicione no array `news`:

```json
{
  "id": 4,
  "date": "2026-05-10",
  "category": "Tech",
  "source": "Fonte da notícia",
  "title_pt": "Título em português",
  "opinion_pt": "Sua opinião aqui"
}
```

---

## 📧 Newsletter (Mailchimp)

1. **Crie conta em** [mailchimp.com](https://mailchimp.com)
2. **Crie uma audience** (lista de emails)
3. **Pegue o Form Action URL** em `Settings` → `Audience` → `Signup forms` → `Embedded forms`
4. **Atualize `config.json`**:
```json
"mailchimp": {
  "enabled": true,
  "formAction": "https://fusion-lab.us8.list-manage.com/subscribe/post?u=SEU_ID&id=SEU_LIST_ID"
}
```

---

## 📊 Google Analytics

1. **Crie conta em** [analytics.google.com](https://analytics.google.com)
2. **Pegue seu Measurement ID** (formato: `G-XXXXXXXXXX`)
3. **Atualize `config.json`**:
```json
"analytics": {
  "googleAnalytics": true,
  "gtag": "G-XXXXXXXXXX"
}
```

---

## 🎨 Google AdSense

1. **Candidato-se em** [adsense.google.com](https://adsense.google.com)
2. **Pegue seu Publisher ID** após aprovação
3. **Atualize `config.json`**:
```json
"googleAdsense": {
  "enabled": true,
  "publisherId": "ca-pub-XXXXXXXXXX"
}
```

Os banners já estão no HTML com placeholders — basta ativar.

---

## 🎯 Próximos passos

- [ ] Configurar Mailchimp newsletter
- [ ] Ativar Google Analytics
- [ ] Candidatar-se ao Google AdSense
- [ ] Adicionar mais posts e notícias
- [ ] Customizar cores e fontes
- [ ] Adicionar imagens de capa
- [ ] Implementar busca local
- [ ] Criar API backend (Node.js/Python)
- [ ] Transformar em CMS headless

---

## 📱 Deploy rápido

### Netlify (5 segundos)
```bash
npm install -g netlify-cli
netlify deploy --prod --dir .
```

### Vercel
```bash
npm install -g vercel
vercel --prod
```

---

## 📄 Licença

MIT — Sinta-se livre para usar, modificar e distribuir.

---

## 🤝 Contato

- LinkedIn: [seu-perfil]
- Twitter: [@seu-handle]
- Email: contato@fusionlab.com

---

**Fusion Lab © 2026** — Construindo ideias que viram forma.
