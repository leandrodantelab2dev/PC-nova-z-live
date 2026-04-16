# A Nova Z — Clean Core na Prática

Página de captura para o evento ao vivo gratuito da Lab2learn sobre ABAP Cloud, Clean Core e desenvolvimento assistido por IA no ecossistema SAP BTP.

---

## Sobre o Projeto

Landing page de alta conversão para captação de leads e inscrições no evento **A Nova Z: Clean Core na Prática**. O design segue uma estética dark/luxury com acentos dourados, otimizado para engajamento e inscrição via e-mail e WhatsApp.

**Data do evento principal:** 16 de maio de 2026, às 9h (horário de Brasília)

---

## Estrutura de Arquivos

```
/
├── index.html       # Página principal de captura
└── obrigado.html    # Página de confirmação pós-inscrição
```

---

## Seções da Página Principal

| Seção | Descrição |
|---|---|
| Hero | Headline, tags de tecnologia, formulário de inscrição e link do grupo WhatsApp |
| Countdown | Timer regressivo em tempo real até o evento |
| O Que Você Vai Aprender | 5 cards com os tópicos abordados |
| Jornada | Timeline dos 5 aquecimentos + evento principal |
| Para Quem É | 4 perfis de público-alvo com checklists |
| CTA Final | Segunda chamada para inscrição e WhatsApp |

---

## Tecnologias e Integrações

### Frontend
- HTML5 / CSS3 / JavaScript vanilla
- Google Fonts — Montserrat (300–900)
- Intersection Observer API para animações de scroll
- Countdown timer com suporte a fuso horário (Brasília)

### Marketing & Analytics
- **RD Station** — Captação de leads via formulário embarcado
  - Form ID: `a-nova-z-ddcd3a6be827d99e9fdc`
  - Loader ID: `2043ecbb-c0bf-46c8-8c5c-2a1c80e7f222`
- **Meta Pixel** — Rastreamento de conversão e retargeting
  - Pixel ID: `1394102987855022`
  - Eventos: `PageView`, `CompleteRegistration`

### Canais de Inscrição
- Formulário de e-mail (RD Station)
- Grupo WhatsApp (link direto)

---

## Design System

| Token | Valor |
|---|---|
| `--preto` | `#0D0D0D` |
| `--carvao` | `#111111` / `#1C1C1C` |
| `--ouro` | `#C9A93B` |
| `--ouro-claro` | `#E5C462` |
| `--creme` | `#F5EFE6` |

**Características visuais:**
- Dark mode com gradientes dourados
- Glassmorphism nos cards de formulário
- Animações orbitais e glow no hero
- Scroll reveal com Intersection Observer
- Totalmente responsivo (breakpoints: 960px e 640px)

---

## Conteúdo do Evento

**Tópicos abordados:**
- Fundamentos do Clean Core no SAP BTP
- Desenvolvimento com ABAP Cloud e RAP (RESTful ABAP Programming Model)
- AI-assisted development no ecossistema SAP
- Arquitetura de extensibilidade cloud-ready
- Boas práticas para projetos SAP modernos

**Público-alvo:**
- Desenvolvedor ABAP em transição para o cloud
- Consultor funcional com interesse técnico
- Arquiteto SAP
- Tech Lead / Gerente de Projetos SAP

---

## Como Rodar Localmente

O projeto é estático — basta abrir `index.html` em um navegador ou servir com qualquer servidor HTTP local:

```bash
# Opção 1: Python
python3 -m http.server 8080

# Opção 2: Node.js (npx)
npx serve .
```

Acesse em `http://localhost:8080`.

> Os formulários RD Station só funcionam corretamente em domínio configurado na conta — em localhost a captura de lead não será registrada.

---

## Deploy

O projeto não requer build. Faça o upload dos arquivos HTML para qualquer hosting estático (Netlify, Vercel, S3, servidor próprio).

---

## Lab2learn

Projeto desenvolvido por **Dante — Lab2Dev** para a formação SAP Cloud da [Lab2learn](https://lab2learn.com.br).
