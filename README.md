# 🔗 Conexão Segura entre Google Colab e Banco de Dados SQL

Este repositório traz um template para você conectar seu notebook do **Google Colab** a um banco de dados **PostgreSQL** (ou outro SQL) de forma segura, sem expor suas credenciais no código.

## 🚀 Funcionalidades

- Conexão com bancos SQL diretamente do Google Colab.
- Armazenamento seguro de credenciais usando um arquivo `.env` no Google Drive.
- Retorno das queries em formato de DataFrame (Pandas) para análises, dashboards ou automações.
- Código modular e fácil de adaptar para outros bancos (MySQL, SQL Server, etc.).

## 🔐 Por que usar arquivo `.env`?

✔️ Protege suas credenciais de acesso (usuário, senha, host, porta, database).  
✔️ Permite versionar e compartilhar notebooks com segurança.  
✔️ Melhora as boas práticas em projetos de ciência de dados, engenharia de dados e automação.

## 📦 Tecnologias e Bibliotecas

- Google Colab  
- Python  
- SQLAlchemy  
- Psycopg2 (PostgreSQL)  
- python-dotenv  
- Pandas  

## 📄 Estrutura do Notebook

1. Montagem do Google Drive.  
2. Instalação das bibliotecas necessárias.  
3. Carregamento seguro das credenciais via `.env`.  
4. Criação do engine de conexão SQL.  
5. Execução de queries SQL e retorno dos dados como DataFrame.  

## 🏗️ Estrutura do Arquivo `.env`

Exemplo do seu arquivo `.env` (NUNCA compartilhe isso publicamente):

```env
DB_USER=seu_usuario
DB_PASS=sua_senha
DB_HOST=seu_host
DB_PORT=sua_porta
DB_NAME=seu_banco
