# 📋 Kanban Bootstrap

Uma aplicação de quadro Kanban interativa, moderna e leve, desenvolvida com **[Astro](https://astro.build/)** e estilizada com **[Bootstrap 5](https://getbootstrap.com/)**.

Possui suporte nativo a **Drag & Drop (HTML5)** sem a necessidade de bibliotecas externas pesadas, permitindo mover tarefas entre colunas e adicionar novos cards através de um modal intuitivo.

---

## ✨ Funcionalidades

- 📌 **Quadro Kanban com 4 Colunas:**
  - **A Fazer** (`todo`)
  - **Em Andamento** (`doing`)
  - **Em Revisão** (`review`)
  - **Concluído** (`done`)
- 🔄 **Drag and Drop Nativo (HTML5):**
  - Arraste e solte cards entre colunas ou reorganize-os dentro da mesma lista.
  - Indicador visual (*placeholder*) para inserção precisa do card.
- 🏷️ **Níveis de Prioridade:**
  - 🔴 **Alta** (destaque vermelho)
  - 🟠 **Média** (destaque laranja)
  - 🟢 **Baixa** (destaque verde)
- ➕ **Criação de Tarefas:**
  - Modal Bootstrap para cadastro de novas tarefas com título, nível de prioridade e coluna de destino.
  - Validação de formulário integrada.
- 🔢 **Contadores Dinâmicos:**
  - Badges informativos nos cabeçalhos de cada coluna com a quantidade de tarefas em tempo real.
- 📱 **Design Responsivo e Moderno:**
  - Tipografia *Plus Jakarta Sans* e ícones com *Bootstrap Icons*.
  - Scroll horizontal fluido para manter a organização em telas menores.
- 🔌 **Pronto para Integração Backend:**
  - Estrutura pronta para disparar requisições assíncronas (REST API, endpoints de persistência, etc.) ao movimentar ou criar cards.

---

## 🚀 Tecnologias Utilizadas

- **[Astro](https://astro.build/)** - Framework web moderno focado em performance.
- **[Bootstrap 5.3](https://getbootstrap.com/)** - Framework CSS para componentes e layout responsivo.
- **[Bootstrap Icons](https://icons.getbootstrap.com/)** - Conjunto de ícones vetoriais.
- **JavaScript Vanilla (ES6+)** - Manipulação de DOM e API nativa de Drag and Drop.
- **HTML5 & CSS3** - Estruturação e estilizações customizadas.

---

## 📁 Estrutura do Projeto

```text
kanban-bootstrap/
├── public/                # Arquivos estáticos (favicons, etc.)
├── src/
│   ├── components/
│   │   ├── Kanban.astro   # Componente principal do quadro e lógica Drag & Drop
│   │   ├── Modal.astro    # Modal Bootstrap para inclusão de novas tarefas
│   │   └── style.css      # Estilização do quadro, colunas, cards e placeholders
│   ├── layouts/
│   │   └── Layout.astro   # Template base (meta tags, fontes e scripts do Bootstrap)
│   └── pages/
│       └── index.astro    # Página inicial da aplicação
├── package.json           # Dependências e scripts do projeto
├── astro.config.mjs       # Configurações do Astro
└── README.md              # Documentação do projeto
```

---

## 🛠️ Como Executar o Projeto

### Pré-requisitos

- **Node.js**: `>= 22.12.0` (recomendado) ou versão LTS atual.
- Gerenciador de pacotes **npm** (ou `pnpm` / `yarn`).

### Instalação e Execução

1. Clone o repositório:
   ```bash
   git clone https://github.com/rogeriosaraceni/kanban-bootstrap.git
   cd kanban-bootstrap
   ```

2. Instale as dependências:
   ```bash
   npm install
   ```

3. Inicie o servidor de desenvolvimento:
   ```bash
   npm run dev
   ```

4. Acesse no navegador:
   ```
   http://localhost:4321
   ```

---

## 🧞 Scripts Disponíveis

| Comando | Descrição |
| :--- | :--- |
| `npm run dev` | Inicia o servidor local de desenvolvimento em `localhost:4321` |
| `npm run build` | Compila o projeto otimizado para produção no diretório `./dist/` |
| `npm run preview` | Executa uma prévia local do build de produção |
| `npm run astro ...` | Executa comandos da CLI do Astro (ex: `astro check`) |

---

## 📄 Licença

Este projeto está sob a licença [MIT](LICENSE).
