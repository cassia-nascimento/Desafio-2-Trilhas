<h1 align="center">
  🔐 Sistema de Autenticação & Fluxo de Usuários
  <br>
  Desafio 2 Trilhas Inova
</h1>

<p align="center">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/Trilhas%20Inova-Desafio%202-brightgreen?style=for-the-badge" alt="Trilhas Inova">
</p>

Repositório dedicado à resolução do **Segundo Desafio Prático** proposto pelo programa **Trilhas Inova Maranhão**. A aplicação consiste em um sistema modularizado client-side que orquestra telas de login, recuperação de credenciais, formulários avançados de cadastro de perfis e uma área administrativa de listagem dinâmica.

<p align="center"> <img src="assets/tela-inicial.png" alt="Tela Inicial" width="90%"> </p>

---

## 📌 Arquitetura de Fluxo & Regras de Negócio

O motor lógico do sistema (dividido de forma modular entre os arquivos da pasta `js/`) gerencia a persistência volátil e a interface adotando conceitos consolidados de desenvolvimento web:

* **Modularidade de Interfaces (Rotas Estáticas):** O ecossistema é composto por 5 visualizações interdependentes (`login.html`, `alterar-senha.html`, `index.html`, `forms.html` e `info-usuarios.html`), simulando a árvore de navegação de um software corporativo real.
* **Interceptação e Validação de Formulários (`form.js`):** Implementação de ouvintes de eventos (*Event Listeners*) que interceptam o envio de dados. O JavaScript realiza a sanitização de strings, valida formatos obrigatórios e bloqueia o comportamento padrão do navegador (`event.preventDefault()`) caso existam inconsistências lógicas nos campos.
* **Gerenciamento de Estado Client-Side:** Fluxo automatizado de dados onde os perfis capturados nos formulários alimentam arrays estruturados na memória de execução da página. A tela `info-usuarios.html` lê reativamente essas coleções para gerar novos nós e cartões no DOM em tempo real.
* **UX/UI Responsiva de Alto Impacto:** Estilização centralizada em `style/style.css` utilizando propriedades modernas de posicionamento (CSS Grid e Flexbox), garantindo que os formulários de onboarding, o painel de usuários e os modais de feedback adaptem-se fluidamente a dispositivos móveis e desktops.

---

## 📂 Estrutura do Repositório

```text
desafio-2-trilhas
├── assets/             # Ilustrações vetoriais (SVGs), ícones de alerta e frames visuais
├── js/
│   ├── login.js        # Lógica de controle de acessos e recuperação de credenciais
│   └── form.js         # Inteligência de validação de inputs e renderização de perfis
├── style/
│   └── style.css       # Design System unificado, tokens de cores e layouts responsivos
├── index.html          # Portal inicial da aplicação
├── login.html          # Interface de autenticação segura simbólica
├── alterar-senha.html  # Fluxo de redefinição de chaves de usuário
├── forms.html          # Formulário estruturado de cadastro de dados
└── info-usuarios.html  # Dashboard administrativo de listagem de perfis cadastrados

```

---

## 🚀 Como Executar o Projeto

Por se tratar de uma aplicação front-end nativa pura (client-side), ela executa de forma imediata no navegador sem a necessidade de contêineres, servidores ou interpretadores de terminal:

1. Realize o clone deste repositório em sua máquina:
```bash
git clone https://github.com/cassia-nascimento/desafio-2-trilhas.git

```


2. Acesse a pasta raiz do projeto:
```bash
cd desafio-2-trilhas

```


3. Abra o arquivo `login.html` diretamente em seu navegador web de preferência (Chrome, Firefox, Safari ou Edge) para iniciar o fluxo completo do sistema.

---

## 👩‍💻 Autoras

Projeto construído, arquitetado e documentado em colaboração por:

| Desenvolvedora | GitHub | LinkedIn |
| :--- | :--- | :--- |
| **Cássia Nascimento** | [@cassia-nascimento](https://github.com/cassia-nascimento) | [In/cassia--nascimento](https://www.linkedin.com/in/cassia--nascimento/) |
| **Sthefane Silva** | [@sthedsyl](https://github.com/sthedsyl) | [In/sthefane-silva](https://www.linkedin.com/in/sthefane-silva-10b194279/) |

---

Projeto desenvolvido durante o programa Trilhas 2B (Trilhas Inova Maranhão).
