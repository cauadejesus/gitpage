# Site criado para mostrar meu portfólio

## Link do site
- A URL pública é: https://cauadejesus.github.io/gitpage/dist/index.html

# 🚀 PortfolioHUB

Plataforma centralizada para exibição, gerenciamento e versionamento de projetos e portfólios digitais, desenvolvida como entrega final da disciplina de Bootcamp do curso de Ciência da Computação.

O desenvolvimento e a implantação desta plataforma foram guiados de ponta a ponta utilizando o **Google GEMINI** como inteligência artificial de apoio estratégico, atuando como co-piloto na arquitetura, segurança e governança do código.

---

## 🗺️ 1. Planejamento da Implantação

A implantação do PortfolioHUB seguiu um cronograma ágil estruturado entre os dias 08/06/2026 e 14/06/2026, com os seguintes marcos de execução (*milestones*):

*   **Fase 1: Configuração e Integração (09/06):** Limpeza e estruturação do ambiente do repositório existente (`gitpage`) e mapeamento do armazenamento de projetos.
*   **Fase 2: Gestão de Usuários e Segurança (10/06):** Configuração de regras de proteção de branch e auditoria de vulnerabilidades[cite: 3].
*   **Fase 3: Governança e Colaboração (11/06):** Formalização do fluxo de trabalho em equipe no arquivo global de documentação[cite: 3].
*   **Fase 4: Testes de Produção (12/06):** Homologação de links, responsividade no GitHub Pages e integridade dos scripts de build[cite: 2, 3].
*   **Fase 5: Lançamento e Apresentação (13/06 a 14/06):** Finalização dos relatórios técnicos e gravação da apresentação oficial para o YouTube[cite: 3].

---

## 🛠️ 2. Arquitetura e Estrutura do Repositório

O projeto adota uma arquitetura de compilação moderna e automatizada via scripts Node.js. A árvore de diretórios está organizada da seguinte forma[cite: 3]:

*   `📂 src/`: Contém os arquivos fontes originais e estruturais da aplicação (Pug, SCSS, JS modular).
*   `📂 scripts/`: Scripts de automação local para tarefas de limpeza e build (`clean.js`, `render-assets.js`, `build-scss.js`, etc.).
*   `📂 dist/`: Pasta de distribuição compilada que abriga os arquivos finais estáticos de produção lidos pelo servidor web do GitHub Pages (`index.html`, `projects.html`, `resume.html`, `contact.html`)[cite: 2, 3].
    *   `📂 dist/assets/`: Armazenamento de mídias e comprovações de entregas do ecossistema, como o `PortifólioHub.pdf`, `curriculum.pdf`, e as capturas de tela dos projetos (`fakeflix.png`, `android_site.png`)[cite: 1, 3].

> ⚠️ **Aviso importante:** Nunca altere diretamente os arquivos contidos na pasta `/dist`. Qualquer modificação de layout ou conteúdo deve ser codificada na pasta `/src` e compilada através dos scripts oficiais mapeados no `package.json`[cite: 3].

---

## 🔒 3. Gestão de Usuários, Acesso e Segurança

Para mitigar riscos de integridade e garantir conformidade com as melhores práticas de engenharia de software monitoradas pelo Google GEMINI, as seguintes políticas de segurança estão ativas no ambiente GitHub[cite: 3]:

### 3.1 Descarte e Blindagem de Arquivos (`.gitignore`)
O arquivo `.gitignore` na raiz do projeto está configurado para blindar o repositório contra upload acidental de arquivos desnecessários ou credenciais sensíveis, incluindo obrigatoriamente[cite: 3]:
*   `node_modules/` (Módulos de dependências locais do Node.js).
*   `.env` (Variáveis de ambiente locais e chaves privadas).
*   Arquivos temporários e logs de erro do sistema (`.DS_Store`, `npm-debug.log`).

### 3.2 Proteção de Branches (*Branch Protection Rules*)
*   A branch principal (`main` / `master`) está configurada sob **regra de proteção estrita**[cite: 3].
*   Commits diretos e pushes não autorizados na branch de produção são bloqueados pelo GitHub[cite: 3].
*   A inserção de qualquer linha de código só é permitida após a abertura, revisão e aprovação formal de um **Pull Request (PR)**[cite: 3].

### 3.3 Análise Automatizada de Código
*   **Dependabot Alerts:** Monitoramento contínuo das dependências declaradas no `package.json` para correção automática de pacotes vulneráveis[cite: 3].
*   **Secret Scanning:** Varredura nativa do GitHub ativa para bloquear a publicação de chaves públicas textuais de segurança de forma despropositada.

---

## 🤝 4. Compartilhamento e Práticas de Colaboração (Git Workflow)

Para permitir colaborações limpas, seguras e versionadas de outros estudantes ou desenvolvedores sem quebrar o ambiente de produção, adote estritamente o seguinte fluxo de trabalho[cite: 3]:

### Passo 1: Fork e Clone
1. Faça um **Fork** deste repositório oficial para a sua conta pessoal do GitHub.
2. Clone o seu fork localmente em sua máquina de trabalho:
```bash
   git clone [https://github.com/SEU_USUARIO/gitpage.git](https://github.com/SEU_USUARIO/gitpage.git)
