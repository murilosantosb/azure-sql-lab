# ☁️ Criando um Banco de Dados SQL no Azure

## 📌 Descrição do Projeto

Este projeto tem como objetivo demonstrar o processo de criação e configuração de um banco de dados SQL utilizando a plataforma **Microsoft Azure**.

Durante o desafio foram explorados conceitos fundamentais de **computação em nuvem**, incluindo a criação de recursos, configuração de servidores SQL e gerenciamento de banco de dados através do **Azure Portal**.

O projeto faz parte de um laboratório prático voltado ao aprendizado de **infraestrutura em nuvem e gerenciamento de dados**.

---

# 🎯 Objetivos

* Compreender o funcionamento do **Azure SQL Database**
* Criar um banco de dados na nuvem utilizando o **Azure Portal**
* Configurar um **SQL Server lógico**
* Conectar ao banco de dados e executar comandos SQL
* Documentar todo o processo utilizando **GitHub**

---

# 🛠️ Tecnologias Utilizadas

* Microsoft Azure
* Azure SQL Database
* SQL
* GitHub
* Markdown

---

# ☁️ Etapas Realizadas

## 1️⃣ Acesso ao Portal do Azure

Primeiramente foi realizado o acesso ao portal da Microsoft Azure:

https://portal.azure.com

Após o login, foi possível acessar o painel principal para criação de recursos na nuvem.

---

## 2️⃣ Criação do Recurso SQL Database

Dentro do portal foi selecionada a opção:

Create a resource → SQL Database → Create

Nessa etapa foram definidas as informações básicas do banco de dados.

**Configurações utilizadas:**

* Database name: `db_exemplo`
* Resource Group: `rg-lab-sql`
* Server: novo servidor criado

---

## 3️⃣ Criação do Servidor SQL

Foi necessário criar um **SQL Server lógico** para hospedar o banco de dados.

Configurações utilizadas:

* Server name: `sqlserver-lab`
* Region: Brazil South
* Admin login: `adminuser`
* Authentication: SQL Authentication

Esse servidor será responsável por gerenciar os bancos de dados criados dentro dele.

---

## 4️⃣ Configuração de Desempenho

Na aba **Compute + Storage**, foi selecionado um plano adequado para estudos.

Exemplo de configuração:

* Tier: Basic
* Compute: baixo consumo
* Storage: padrão

Essa configuração é suficiente para ambientes de laboratório.

---

## 5️⃣ Configuração de Rede

Foi habilitado o acesso público ao banco de dados.

Configuração utilizada:

Public Endpoint habilitado
Allow Azure services and resources to access this server

Isso permite a conexão com ferramentas externas ou diretamente pelo portal.

---

## 6️⃣ Criação do Banco de Dados

Após revisar todas as configurações, foi selecionada a opção:

Review + Create → Create

O Azure realizou o **deploy do banco de dados**, finalizando a criação do ambiente.

---

# 🧪 Teste do Banco de Dados

Após a criação, foi utilizado o **Query Editor do Azure** para executar comandos SQL.

Exemplo de criação de tabela:

```sql
CREATE TABLE clientes (
    id INT PRIMARY KEY,
    nome VARCHAR(100),
    email VARCHAR(100)
);
```

Inserindo dados de teste:

```sql
INSERT INTO clientes VALUES
(1, 'Murilo', 'murilo@email.com');
```

Consulta dos dados:

```sql
SELECT * FROM clientes;
```

---

# 📸 Evidências do Projeto

As capturas de tela do processo estão disponíveis na pasta:

```
/images
```

Exemplos de imagens incluídas:

* Criação do recurso SQL Database
* Configuração do servidor
* Deploy do banco de dados
* Execução de comandos SQL

---

# 📚 Aprendizados

Durante a realização deste desafio foi possível aprender:

* Como criar recursos na plataforma Azure
* Estrutura de um banco de dados SQL na nuvem
* Configuração de servidores SQL no Azure
* Execução de comandos SQL diretamente no portal
* Documentação técnica utilizando GitHub

---

# 🚀 Conclusão

Este projeto permitiu compreender na prática como funciona a criação e gerenciamento de um banco de dados em ambiente de **cloud computing**.

A utilização do **Azure SQL Database** demonstra como serviços gerenciados podem facilitar o desenvolvimento de aplicações escaláveis e seguras.

---

# 🔗 Referências

Documentação oficial da Microsoft:

https://learn.microsoft.com/azure/azure-sql/database/

---
