# KatoDevCoffee — Documentação do Projeto

> Página centralizada de pagamentos, vitrine de apps e identidade de marca do desenvolvedor.

---

## Visão Geral

O projeto **KatoDevCoffee** é uma landing page profissional que serve como:

1. **Vitrine de Apps** — exibe todos os produtos publicados na Google Play e App Store
2. **Portal de Contribuições** — permite que usuários dos apps apoiem o desenvolvedor via Stripe, Mercado Pago e PayPal
3. **Identidade de Marca** — consolida a presença online do desenvolvedor sob um domínio único e confiável

---

## Estrutura do Projeto

```
KatoDevCoffe/
├── docs/
│   ├── README.md              ← Este arquivo
│   ├── ANALISE_TECNICA.md     ← Análise de viabilidade e tecnologia
│   ├── SKIN_DESIGN.md         ← Guia de design e identidade visual
│   └── CURRICULO.md           ← Currículo resumido do desenvolvedor
├── src/
│   ├── index.html             ← Landing page principal (estático)
│   ├── backend/
│   │   ├── main.py            ← API FastAPI (sessões Stripe)
│   │   └── requirements.txt
│   └── assets/
│       └── icons/             ← Ícones dos apps
└── README.md
```

---

## Apps & Softwares do Portfólio

### FastPDF
- **Plataforma:** Android
- **Descrição:** Aplicativo para leitura, gerenciamento e conversão de documentos PDF no mobile. Focado em leveza, velocidade e experiência offline. Permite visualizar, anotar e compartilhar PDFs diretamente pelo dispositivo Android.
- **Tecnologia:** Kotlin, Android SDK
- **Diferenciais:** Interface limpa, zero propagandas intrusivas, respeito à privacidade do usuário

### [Seus demais apps]
> Adicione aqui os outros aplicativos do portfólio com nome, descrição e link de loja.

---

## Fluxo de Contribuição

```
App Android (menu "Sobre")
        ↓
Botão "Contribua / Buy me a Coffee"
        ↓
Browser abre: katodev.com/contribute?utm_source=fastpdf
        ↓
Usuário escolhe o valor (R$5 / R$10 / R$20 / personalizado)
        ↓
Backend Python cria sessão Stripe
        ↓
Stripe Checkout (seguro, hospedado)
        ↓
Retorno: katodev.com/success
```

---

## Roadmap

- [x] Análise técnica e arquitetura
- [x] Design da página (skin)
- [x] Currículo do desenvolvedor
- [ ] Cadastro no Stripe
- [ ] Deploy (Vercel / Render / Railway)
- [ ] Integração nos apps Android (Intent URL)
- [ ] Domínio personalizado
