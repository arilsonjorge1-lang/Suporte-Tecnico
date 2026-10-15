# 🛠️ Sistema de Chamados & Assistência Técnica

Sistema web completo, leve e responsivo para gestão de chamados de assistência técnica. O projeto conta com um **Portal do Cliente**, **Painel do Técnico**, notificações formatadas no **WhatsApp** com links dinâmicos de acompanhamento e armazenamento local persistente via **localStorage**.

---

## 🚀 Funcionalidades

- **Portal do Cliente:**
  - Formulário intuitivo para abertura de chamados (Empresa, Solicitante, Telefone, Tipo de Problema e Descrição).
  - Tabela de acompanhamento dos chamados já registrados.
  - Painel de busca e visualização direta do estado por ID do ticket.

- **Painel do Técnico:**
  - Visão geral de todos os chamados em aberto.
  - Alteração imediata do status (`🟡 Aberto`, `🔵 Em Andamento`, `🟠 Aguardando Cliente`, `🟢 Resolvido`).
  - Botão de gerenciamento e limpeza total do histórico.

- **Integração com WhatsApp:**
  - Envio automático da notificação formatada para o suporte via WhatsApp (`+238 9930138`).
  - Geração automática de link único por chamado (`#ticket-ID`) dentro da mensagem do WhatsApp para fácil acesso do cliente.

- **Persistência de Dados (`localStorage`):**
  - Armazenamento no próprio navegador. Os chamados e alterações de estado permanecem salvos mesmo após fechar ou recarregar a página.

---

## 💻 Tecnologias Utilizadas

- **HTML5:** Estrutura da aplicação e formulários.
- **CSS3:** Design responsivo, estilização de tabelas, badges de status e layout flex/grid.
- **JavaScript (Vanilla):** Lógica da aplicação, manipulate de DOM, suporte ao `localStorage`, leitura de `hash` da URL e integração com a API do WhatsApp.

---

## 📂 Estrutura do Projeto

```text
.
├── index.html     # Aplicação completa (Interface + Lógica + Estilos)
└── README.md      # Documentação do repositório
```

---

## 🚀 Como Executar o Projeto

1. **Localmente:**
   - Clone este repositório ou faça o download dos arquivos:
     ```bash
     git clone https://github.com/seu-usuario/seu-repositorio.git
     ```
   - Abra o arquivo `index.html` em qualquer navegador web (Chrome, Edge, Firefox, Safari).

2. **Na Nuvem (Hospedagem Gratuita):**
   - **GitHub Pages:**
     1. Acesse **Settings** > **Pages** no seu repositório.
     2. Selecione a *branch* `main` e salve.
     3. O link público da sua aplicação estará disponível em instantes.
   - **Netlify:**
     1. Acesse o [Netlify Drop](https://app.netlify.com/drop).
     2. Arraste a pasta contendo o arquivo `index.html`.

---

## ⚙️ Configurações

Para alterar o número do WhatsApp que recebe as notificações dos novos chamados, edite a seguinte constante no arquivo `index.html`:

```javascript
const SEU_WHATSAPP = "2389930138"; // Código de país + Número de telefone
```

---

## 📄 Licença

Este projeto é open-source e está disponível para uso, modificação e distribuição.