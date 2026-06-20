# Farmácia Vida & Saúde

Landing page de alta conversão para farmácia fictícia, desenvolvida com foco em responsividade, acessibilidade e integração WhatsApp (delivery ou retirada no balcão).

[![Live Demo](https://img.shields.io/badge/demo-online-brightgreen)](https://tofariasti.github.io/landing-farmacia/)

## Demo

**Moldura (preview):** [https://tofariasti.github.io/landing-farmacia/](https://tofariasti.github.io/landing-farmacia/)

**Tela cheia:** [https://tofariasti.github.io/landing-farmacia/site/](https://tofariasti.github.io/landing-farmacia/site/)

## Screenshots

### Desktop (1280px)
![Desktop view](screenshots/desktop.png)

### Tablet (768px)
![Tablet view](screenshots/tablet.png)

### Mobile (390px)
![Mobile view](screenshots/mobile.png)

## Funcionalidades

- Design responsivo (mobile-first)
- Integração WhatsApp com formulário estruturado (delivery ou balcão)
- Ticker animado de ofertas da semana
- Animações ao scroll (AOS) + partículas, contadores e hover em cards
- Grid de ofertas com preço antigo/riscado e badge promocional
- Botão flutuante WhatsApp com pulse ring
- FAQ accordion interativo
- Acessibilidade WCAG 2.1 AA (skip link, ARIA, contraste, foco visível)
- Respeita `prefers-reduced-motion`

## Seções

1. **Hero** — Headline, CTAs, estatísticas e imagem da farmácia
2. **Serviços** — Medicamentos, manipulação, dermocosméticos, vacinas, vitaminas, consulta farmacêutica
3. **Ofertas** — 6 produtos em promoção
4. **Como pedir** — 3 passos do pedido à entrega/retirada
5. **Diferenciais** — Farmacêuticos CRQ, delivery, manipulação, produtos originais
6. **Galeria** — Fotos do interior, laboratório e delivery
7. **Depoimentos** — 3 avaliações de clientes
8. **CTA** — Seção de conversão intermediária
9. **FAQ** — Horário, delivery, manipulação, pagamento
10. **Contato** — Formulário WhatsApp completo
11. **Footer** — Endereço, horários e créditos

## Tecnologias

- HTML5 semântico
- CSS3 (Flexbox/Grid, custom properties)
- JavaScript vanilla (IIFE, ES5+)
- AOS (Animate On Scroll) v2.3.4
- Font Awesome 6.4
- Google Fonts (Playfair Display + Source Sans 3)

## Testes de Responsividade

| Dispositivo | Resolução | Status | Verificado |
|-------------|-----------|--------|------------|
| iPhone SE | 375×667 | ✅ | Menu mobile, formulário, float WhatsApp |
| iPhone 12 Pro | 390×844 | ✅ | Hero, grid ofertas, CTA above the fold |
| iPhone 14 Pro Max | 428×926 | ✅ | Layout mobile amplo, ticker ofertas |
| iPad | 768×1024 | ✅ | Grid 2 colunas, FAQ, serviços |
| Desktop HD | 1280×720 | ✅ | Layout completo, moldura preview |
| Desktop FHD | 1920×1080 | ✅ | Max-width container, galeria 3 colunas |

## Acessibilidade

- Semântica HTML5 (`header`, `main`, `footer`, `nav`, landmarks)
- Skip link para conteúdo principal
- Atributos ARIA (`aria-expanded`, `aria-label`, `role="alert"` em erros)
- Contraste WCAG AA (4.5:1) — verde #0D7A52 sobre branco, laranja #F5A623 em CTAs
- Navegação por teclado (Escape fecha menu mobile)
- Focus states visíveis em todos os interativos
- Alt text descritivo em imagens
- Labels explícitos em formulários
- Font-size mínimo 16px em inputs mobile
- `prefers-reduced-motion`: desabilita AOS, ticker, pulse e partículas

## Como usar

```bash
git clone https://github.com/tofariasti/landing-farmacia.git
cd landing-farmacia
# Abrir index.html no navegador (preview com moldura iframe)
# Ou abrir site/index.html para tela cheia
python3 -m http.server 8080
```

## Screenshots (geração)

```bash
python3 -m http.server 8765
npm install
npm run screenshots
```

## Personalização

1. **WhatsApp:** altere `WHATSAPP_NUMBER` em `site/assets/js/main.js`
2. **Cores:** edite as variáveis CSS em `:root` no `site/assets/css/style.css`
3. **Textos e ofertas:** edite `site/index.html`

## Estrutura

```
farmacia/
├── index.html              # Preview shell (moldura iframe)
├── assets/css/preview.css
├── assets/js/preview.js
├── site/
│   ├── index.html          # Landing page
│   └── assets/
│       ├── css/style.css
│       └── js/main.js
├── screenshots/
├── scripts/capture-screenshots.mjs
├── .github/workflows/deploy.yml
└── README.md
```

## Autor

**Tiago O. de Farias** — [Farias Digital](https://fariasdigital.com.br/)

- GitHub: [@tofariasti](https://github.com/tofariasti)
- WhatsApp: [(51) 99121-3724](https://wa.me/5551991213724)

---

<p align="center">
  <a href="https://tofariasti.github.io/landing-farmacia/">🌐 Demo Online</a> ·
  <a href="https://fariasdigital.com.br/">🏢 Site Comercial</a>
</p>
