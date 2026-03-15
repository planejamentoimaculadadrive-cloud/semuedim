# 🏫 Sistema Pedagógico 2026
> **Gestão inteligente de planos de aula integrados à BNCC.**

![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-brightgreen)
![Tecnologias](https://img.shields.io/badge/Tech-HTML%20%7C%20JS%20%7C%20GAS-blue)

Este sistema foi desenvolvido para modernizar o processo de planejamento pedagógico. Ele permite que professores registrem, consultem e editem seus planos de aula de forma rápida, com armazenamento direto em nuvem via Google Sheets.

---

## 🚀 Funcionalidades Principais

- 🔐 **Acesso Restrito:** Sistema de login validado via base de dados de docentes.
- 📝 **Lançamento Inteligente:** Seleção dinâmica de Áreas, Objetos e Habilidades da BNCC.
- 📅 **Trava de Segurança:** Validação de data (limite de 15 dias retroativos ou futuros).
- ✏️ **Gestão de Registros:** Painel para consulta, edição e exclusão de planos existentes.
- 📊 **Relatórios:** Estrutura preparada para geração de indicadores pedagógicos.

---

## 🛠️ Tecnologias e Arquitetura

O projeto utiliza uma arquitetura **Serverless** simplificada:

* **Frontend:** HTML5, CSS3 (Design Responsivo) e JavaScript Moderno (Fetch API).
* **Backend:** [Google Apps Script](https://www.google.com/script/start/) (Processamento de dados).
* **Banco de Dados:** [Google Sheets](https://www.google.com/sheets/about/) (Armazenamento em tempo real).

---

## ⚙️ Configuração do Backend (Google Apps Script)

Para replicar este ambiente, siga as instruções abaixo:

1.  Crie uma Planilha Google com as abas: `RESPOSTAS`, `CONFIG_SISTEMA`, `REFERENCIAS` e `CADASTRO_DOCENTE`.
2.  No menu **Extensões > Apps Script**, cole o conteúdo do arquivo `Codigo.gs`.
3.  Substitua a constante `SPREADSHEET_ID` pelo ID da sua planilha.
4.  Clique em **Implantar > Nova Implantação**.
    * **Tipo:** App da Web
    * **Quem pode acessar:** Qualquer pessoa
5.  Copie a URL gerada e cole na variável `URL_SCRIPT` dos arquivos HTML.

---

## 📂 Estrutura de Arquivos

```text
├── Login.html        # Tela de acesso inicial
├── Painel.html       # Menu principal do sistema
├── Formulario.html   # Cadastro e Edição de planos
├── Consulta.html     # Visualização e filtros de histórico
├── Codigo.gs         # Lógica do servidor (Google Script)
└── README.md         # Documentação do projeto
