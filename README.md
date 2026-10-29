Landing Page - Milena Araldi

Landing page simples e responsiva para o salão de design de sobrancelhas, cílios e estética facial da proprietária Milena Araldi, construída na plataforma no-code Softr, com um carrossel de serviços feito em low-code (HTML, CSS e JavaScript) inserido em um bloco de código personalizado e integração com um chatbot de agendamento no Telegram, automatizado com o Make.

Acesse o site: https://german59466.softr.app

Agende pelo Telegram: https://t.me/AssistenteMile_bot

Sobre o projeto

O objetivo foi criar uma página de apresentação para o salão, onde a cliente pode conhecer os serviços oferecidos e seus preços de forma rápida e visual, tanto no computador quanto no celular, e já partir direto para o agendamento.

A maior parte da página foi montada com os blocos nativos do Softr. Para a vitrine de serviços, usamos um bloco de código personalizado (Custom Code), o que permitiu criar um carrossel com comportamento e visual sob medida.

A página também conta com uma conexão com um chatbot no Telegram para agendamento, desenvolvido com automações no Make, para que a cliente consiga marcar seu horário de forma prática, sem sair do celular.

Tecnologias utilizadas
Ferramenta	Uso
Softr	Construção e publicação da landing page (no-code)
Softr Tables	Armazenamento das imagens dos serviços
HTML	Estrutura do carrossel
CSS	Layout, cores, responsividade e estilo dos cards
JavaScript	Navegação, bolinhas indicadoras, autoplay e adaptação para mobile
Make	Automação do fluxo de agendamento do chatbot
Telegram	Canal de atendimento e agendamento da cliente (bot)
Funcionalidades do carrossel
3 cards por vez no desktop e tablet, com setas de navegação (‹ ›)
1 card centralizado no celular, com navegação por arraste (setas ocultas)
Responsividade pelo tamanho do bloco, e não da janela (via ResizeObserver), funcionando bem dentro do layout do Softr
Bolinhas indicadoras que mostram o card atual e permitem pular direto para um serviço
Autoplay a cada 4 segundos, voltando ao início ao chegar no último card
Scroll suave com “snap”, para os cards sempre pararem alinhados
Botões com aria-label para melhor acessibilidade
Agendamento via Telegram

A landing page possui um link de acesso ao chatbot de agendamento no Telegram, criado com o Make. Por ele, a cliente pode solicitar e organizar seu atendimento de forma automatizada.

Acesse o bot: @AssistenteMile_bot

Serviços exibidos
Serviço	Preço
Design de Sobrancelhas	R$ 50,00
Henna para Sobrancelhas	R$ 40,00
Micropigmentação Labial	R$ 600,00
Extensão de Cílios Fio a Fio	R$ 150,00
Volume Russo	R$ 220,00
Lash Lifting	R$ 180,00
Limpeza de Pele Profunda	R$ 120,00
Microagulhamento	R$ 350,00
Estrutura do repositório
├── README.md                  # Este arquivo
├── carrossel-servicos.html    # Código low-code do carrossel (HTML + CSS + JS)
└── prints/                    # Capturas de tela da página (desktop e mobile)
Como usar o carrossel no Softr
No editor do Softr, adicione um bloco Custom Code na página.
Cole o conteúdo do arquivo carrossel-servicos.html.
Para trocar um serviço, edite dentro de cada <div class="srv-card">:
o link da imagem em src="..."
o nome em <h3>...</h3>
o preço em <strong>...</strong>
Clique em Publish para atualizar o site.

Dica: para adicionar um novo serviço, basta copiar um bloco srv-card inteiro e colar abaixo dos outros. As bolinhas indicadoras são criadas automaticamente pelo script.
