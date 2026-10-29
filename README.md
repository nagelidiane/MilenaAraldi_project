<h1 align="center">Landing Page - Milena Araldi</h1>

<p align="center">
  Landing page responsiva para salão de design de sobrancelhas, cílios e estética facial,<br>
  com carrossel de serviços em low-code e agendamento automatizado via Telegram.
</p>

<p align="center">
  <a href="https://german59466.softr.app"><img src="https://img.shields.io/badge/Acessar%20o%20site-Softr-6C47FF?style=for-the-badge" alt="Acessar o site"></a>
  <a href="https://t.me/AssistenteMile_bot"><img src="https://img.shields.io/badge/Agendar-Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" alt="Agendar pelo Telegram"></a>
</p>

---

## Sobre o projeto

Página de apresentação para o salão da proprietária **Milena Araldi**, onde a cliente conhece os serviços e os preços de forma rápida e visual, no computador ou no celular, e já pode partir direto para o agendamento.

A maior parte da página foi montada com os blocos nativos do **Softr** (no-code). Para a vitrine de serviços foi usado um bloco de **Custom Code**, que permitiu criar um carrossel com comportamento e visual sob medida (**low-code**: HTML, CSS e JavaScript).

A landing page também possui **conexão com um chatbot no Telegram para agendamento**, desenvolvido com automações no **Make**.

**Site:** https://german59466.softr.app
**Bot de agendamento:** [@AssistenteMile_bot](https://t.me/AssistenteMile_bot)

---

## Tecnologias utilizadas

| Ferramenta | Uso |
|---|---|
| **Softr** | Construção e publicação da landing page (no-code) |
| **Softr Tables** | Armazenamento das imagens dos serviços |
| **HTML** | Estrutura do carrossel |
| **CSS** | Layout, cores, responsividade e estilo dos cards |
| **JavaScript** | Navegação, bolinhas indicadoras, autoplay e adaptação para mobile |
| **Make** | Automação do fluxo de agendamento do chatbot |
| **Telegram** | Canal de atendimento e agendamento da cliente (bot) |

---

## Funcionalidades do carrossel

- **3 cards por vez** no desktop e tablet, com setas de navegação (‹ ›)
- **1 card centralizado** no celular, com navegação por arraste (setas ocultas)
- **Responsividade pelo tamanho do bloco**, e não da janela (via `ResizeObserver`), funcionando bem dentro do layout do Softr
- **Bolinhas indicadoras** que mostram o card atual e permitem pular direto para um serviço
- **Autoplay** a cada 4 segundos, voltando ao início ao chegar no último card
- **Scroll suave com "snap"**, para os cards sempre pararem alinhados
- Botões com `aria-label` para melhor acessibilidade

---

## Agendamento via Telegram

A landing page possui um link de acesso ao **chatbot de agendamento no Telegram**, criado com o **Make**. Por ele, a cliente pode solicitar e organizar seu atendimento de forma automatizada, sem sair do celular.

**[Abrir o bot @AssistenteMile_bot](https://t.me/AssistenteMile_bot)**

---

## Serviços exibidos

| Serviço | Preço |
|---|---|
| Design de Sobrancelhas | R$ 50,00 |
| Henna para Sobrancelhas | R$ 40,00 |
| Micropigmentação Labial | R$ 600,00 |
| Extensão de Cílios Fio a Fio | R$ 150,00 |
| Volume Russo | R$ 220,00 |
| Lash Lifting | R$ 180,00 |
| Limpeza de Pele Profunda | R$ 120,00 |
| Microagulhamento | R$ 350,00 |

---

## Estrutura do repositório

```
├── README.md                  # Este arquivo
├── carrossel-servicos.html    # Código low-code do carrossel (HTML + CSS + JS)
└── prints/                    # Capturas de tela da página (desktop e mobile)
```

---

## Como usar o carrossel no Softr

1. No editor do Softr, adicione um bloco **Custom Code** na página.
2. Cole o conteúdo do arquivo `carrossel-servicos.html`.
3. Para trocar um serviço, edite dentro de cada `<div class="srv-card">`:
   - o link da imagem em `src="..."`
   - o nome em `<h3>...</h3>`
   - o preço em `<strong>...</strong>`
4. Clique em **Publish** para atualizar o site.

> **Dica:** para adicionar um novo serviço, basta copiar um bloco `srv-card` inteiro e colar abaixo dos outros. As bolinhas indicadoras são criadas automaticamente pelo script.
