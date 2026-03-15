# 🏫 Sistema Pedagógico 2026

Este é um sistema de gestão educacional desenvolvido para facilitar o registro de planos de aula, alinhado às normas da **BNCC**. O projeto utiliza tecnologias web para o frontend e o **Google Sheets** como banco de dados (Backend).

## 🚀 Funcionalidades

* **Login Seguro:** Acesso restrito via Cadastro Docente.
* **Lançamento de Planos:** Formulário inteligente com filtros automáticos da BNCC.
* **Trava de Segurança:** Bloqueio automático para registros fora da janela de 15 dias.
* **Consulta e Edição:** Histórico completo de planos lançados com opção de alteração e exclusão.
* **Banco de Dados:** Integração total com Google Apps Script.

## 🛠️ Tecnologias Utilizadas

* **Frontend:** HTML5, CSS3 (Responsivo) e JavaScript (Async/Await).
* **Backend:** Google Apps Script (GAS).
* **Database:** Google Sheets (Planilhas Google).

## 📋 Pré-requisitos para Instalação

Para rodar este projeto, você precisará:
1. Uma planilha Google configurada com as abas: `RESPOSTAS`, `CONFIG_SISTEMA`, `REFERENCIAS` e `CADASTRO_DOCENTE`.
2. O ID da sua planilha configurado no arquivo `Código.gs`.
3. O URL da Implantação do Script atualizado nos arquivos HTML.

## 🔧 Como Usar

1.  Abra o arquivo `Login.html`.
2.  Insira suas credenciais cadastradas na aba `CADASTRO_DOCENTE`.
3.  No Painel Principal, selecione "Novo Planejamento".
4.  Preencha os dados e clique em "Salvar".