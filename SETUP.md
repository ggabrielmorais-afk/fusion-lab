# Fusion Lab — Setup Completo ✅

## 🎉 Tudo foi configurado!

Aqui está o resumo do que foi criado:

### 📁 Arquivos Adicionados

1. **`data.json`** — Base de dados centralizada
   - 4 posts de exemplo
   - 3 notícias de exemplo
   - 3 ferramentas recomendadas

2. **`config.json`** — Configurações do projeto
   - Mailchimp setup
   - Google Analytics
   - Google AdSense

3. **`.github/workflows/deploy.yml`** — Deploy automático
   - Faz push automático para GitHub Pages

4. **`index.html`** (atualizado) — Carregamento dinâmico
   - Lê posts de `data.json`
   - Lê notícias de `data.json`
   - Newsletter funcional
   - Compartilhamento social

---

## 🚀 Próximas ações (5-10 minutos)

### 1️⃣ Ativar GitHub Pages
```bash
# Vá para Settings → Pages
# Branch: main
# Folder: root (/)
# Save
```
→ Site estará em: `https://ggabrielmorais-afk.github.io/fusion-lab`

### 2️⃣ Configurar Newsletter (Mailchimp)
1. Acesse [mailchimp.com](https://mailchimp.com)
2. Crie uma conta gratuita
3. Vá para **Audience** → **Signup forms** → **Embedded forms**
4. Copie o `<form action="...">`
5. Pegue a URL e atualize `config.json`:
```json
"mailchimp": {
  "formAction": "https://fusion-lab.us8.list-manage.com/subscribe/post?u=AQUI&id=AQUI"
}
```

### 3️⃣ Google Analytics (opcional)
1. Vá para [analytics.google.com](https://analytics.google.com)
2. Crie propriedade "Fusion Lab"
3. Copie o Measurement ID (G-XXXXXXXXXX)
4. Atualize em `index.html` (linha ~15):
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=SEU_ID"></script>
```

### 4️⃣ Google AdSense (opcional)
1. Candidato-se em [adsense.google.com](https://adsense.google.com)
2. Após aprovação, pegue seu Publisher ID
3. Atualize em `index.html` (linha ~17):
```html
<!-- <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-AQUI"></script> -->
```

---

## 📝 Como adicionar conteúdo

### Novo post
Edite `data.json` e adicione ao array `posts`:
```json
{
  "id": 5,
  "slug": "novo-post",
  "category": "Arquitetura",
  "categoryEn": "Architecture",
  "categoryEs": "Arquitectura",
  "categoryColor": "ca",
  "title_pt": "Seu título aqui",
  "title_en": "Your title here",
  "title_es": "Su título aquí",
  "excerpt_pt": "Resumo breve",
  "excerpt_en": "Brief summary",
  "excerpt_es": "Resumen breve",
  "date": "2026-05-15",
  "readTime": 8,
  "views": 0,
  "likes": 0
}
```

### Nova notícia
Edite `data.json` e adicione ao array `news`:
```json
{
  "id": 4,
  "date": "2026-05-15",
  "category": "Tech",
  "categoryColor": "bpt",
  "source": "Nome da fonte",
  "title_pt": "Título em português",
  "title_en": "Title in English",
  "title_es": "Título en español",
  "summary_pt": "Resumo...",
  "summary_en": "Summary...",
  "summary_es": "Resumen...",
  "opinion_pt": "Sua opinião",
  "opinion_en": "Your opinion",
  "opinion_es": "Tu opinión",
  "link": "https://fonte.com/noticia"
}
```

---

## 🎨 Cores disponíveis

Posts:
- `ca` = Amarelo (#C8FF57) — Arquitetura
- `ct` = Azul (#57C8FF) — Tech
- `ce` = Laranja (#FF8A57) — Empreendedorismo
- `cp` = Roxo (#C857FF) — Pessoal

Notícias:
- `bpa` = Amarelo — Arquitetura
- `bpt` = Azul — Tech
- `bpe` = Laranja — Empreendedorismo

---

## ✨ Features já implementadas

✅ Carregamento dinâmico de posts  
✅ Carregamento dinâmico de notícias  
✅ 3 idiomas (PT, EN, ES)  
✅ Newsletter com validação  
✅ Compartilhamento WhatsApp  
✅ Responsive design  
✅ Navegação fluida  
✅ CSS otimizado  
✅ GitHub Actions workflow  

---

## 🔗 Links úteis

- [GitHub Pages Setup](https://pages.github.com/)
- [Mailchimp Free Plan](https://mailchimp.com/pricing/)
- [Google Analytics](https://analytics.google.com/)
- [Google AdSense](https://adsense.google.com/)
- [GitHub Actions](https://github.com/features/actions)

---

## 📞 Suporte

Se precisar de ajuda:
1. Verifique o console do navegador (F12)
2. Verifique se `data.json` está válido (use [jsonlint.com](https://jsonlint.com/))
3. Verifique a URL do seu site

---

**Tudo pronto para começar! 🎉**

Agora você pode:
1. Editar `data.json` com seus posts
2. Fazer push (GitHub Pages atualiza automaticamente)
3. Configurar newsletter e analytics
4. Começar a publicar!

Boa sorte! 🚀
