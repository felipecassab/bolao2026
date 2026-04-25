# ⚽ Bolão Copa 2026 — PWA

App de bolão para Copa do Mundo 2026, funciona no iPhone e Android como app instalável.

## 📁 Estrutura dos arquivos

```
bolao2026/
├── index.html       ← App principal
├── manifest.json    ← Configuração do PWA
├── sw.js            ← Service Worker (funciona offline)
└── icons/
    ├── icon-192.png ← Ícone do app
    └── icon-512.png ← Ícone do app (grande)
```

---

## 🚀 Como hospedar GRATUITAMENTE no Netlify (mais fácil)

1. Acesse [netlify.com](https://netlify.com) e crie uma conta gratuita
2. Na tela inicial, **arraste a pasta `bolao2026`** direto para o site
3. O Netlify gera um link tipo `https://seu-bolao.netlify.app`
4. Pronto! Compartilhe o link com seus amigos

---

## 🐙 Como hospedar no GitHub Pages (gratuito)

1. Crie uma conta em [github.com](https://github.com)
2. Crie um repositório novo (ex: `bolao2026`)
3. Faça upload de todos os arquivos da pasta `bolao2026`
4. Vá em **Settings → Pages → Branch: main → Save**
5. Seu link será: `https://seunome.github.io/bolao2026`

---

## 📱 Como instalar no celular

### iPhone (Safari):
1. Abra o link no Safari
2. Toque no botão **Compartilhar** (quadrado com seta ↑)
3. Selecione **"Adicionar à Tela de Início"**
4. Toque em **Adicionar**

### Android (Chrome):
1. Abra o link no Chrome
2. Aparecerá um banner **"Instalar app"** — toque nele
3. Ou toque nos 3 pontos → **"Adicionar à tela inicial"**

---

## 🎮 Como funciona

- **Palpites**: cada pessoa entra com seu nome e preenche os placares
- **Ranking**: atualizado em tempo real com a pontuação de todos
- **Histórico**: veja quem acertou o quê em cada jogo
- **Quiz**: teste seu conhecimento sobre a Copa

### Pontuação:
- ✅ Placar exato: **3 pontos**
- 🟡 Acertou o vencedor: **1 ponto**  
- ❌ Errou: **0 pontos**

---

## ✏️ Como adicionar mais jogos

Abra o `index.html` e edite o array `MATCHES` lá no início do `<script>`:

```javascript
{id:'m7', home:'Coreia do Sul', away:'Gana', fH:'🇰🇷', fA:'🇬🇭',
 group:'D', status:'upcoming', date:'14 Jun'},
```

Para marcar um jogo como encerrado:
```javascript
{id:'m3', ..., status:'done', rH:2, rA:1},
//                             ↑ gols do time da casa
//                                  ↑ gols do visitante
```

---

Feito com ❤️ para a Copa 2026 🏆
