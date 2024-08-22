# Projeto de Banco de Dados: Comandos de SQL

Este projeto demonstra o uso básico de comandos SQL para criar e manipular um banco de dados. O banco de dados criado é chamado `comandos_10` e contém uma tabela chamada `vendas`.

## Estrutura do Projeto

1. **Criação do Banco de Dados**
   - `CREATE DATABASE comandos_10;`

2. **Seleção do Banco de Dados**
   - `USE comandos_10;`

3. **Criação da Tabela `vendas`**
   - A tabela contém as seguintes colunas:
     - `Id_vendas` (INT): Identificador da venda.
     - `Curso` (VARCHAR(100)): Nome do curso.
     - `Aluno` (VARCHAR(100)): Nome do aluno.
     - `Estado` (VARCHAR(100)): Estado onde o aluno reside.
     - `Valor` (DECIMAL(10, 2)): Valor da venda.

   ```sql
   CREATE TABLE vendas(
     Id_vendas INT,
     Curso VARCHAR(100),
     Aluno VARCHAR(100),
     Estado VARCHAR(100),
     Valor DECIMAL(10, 2)
   );
4.Inserção de Dados

Adiciona registros à tabela vendas.
INSERT INTO vendas(Id_Vendas, Curso, Aluno, Estado, Valor)
VALUES
(1, 'Excel', 'JOÃO', ' SP', 100),
(2, 'VBA', 'LUCAS', 'RJ', 50),
(3, 'EXCEL', 'ALICE', 'SP', 100),
(4, 'EXCEL', 'PEDRO', 'PE', 100),
(5, 'VBA', 'AMANDA', 'BA', 50),
(6, 'POWER BI', 'RITA', 'RS', 80),
(7, 'EXCEL', 'JULIA', 'RJ', 100),
(8, 'POWER BI', 'CAIO', 'SP', 80),
(9, 'POWER BI', 'LARA', 'MG', 80),
(10, 'EXCEL', 'ROGERIO', 'AC', 100);
5.Consultas e Manipulação de Dados

Selecionar Dados
SELECT * FROM vendas;
SELECT aluno, curso, valor FROM vendas;
Ordenar Dados
SELECT * FROM vendas 
ORDER BY id_vendas;
Filtrar Dados
SELECT * FROM vendas
WHERE estado = 'RJ';
Atualizar Dados
UPDATE vendas 
SET valor = 150
WHERE curso = 'VBA';
Excluir Linhas
DELETE FROM vendas
WHERE ID_vendas = 10;
Excluir Todos os Dados
TRUNCATE TABLE vendas;
Como Executar
Configuração do Ambiente

Certifique-se de que você tem um sistema de gerenciamento de banco de dados SQL instalado, como MySQL ou MariaDB.
Execução dos Comandos

Copie e cole os comandos SQL fornecidos no seu cliente SQL para criar o banco de dados, a tabela e manipular os dados.
Contribuições
Sinta-se à vontade para contribuir com melhorias para este projeto. Se você encontrar erros ou tiver sugestões, envie uma pull request ou abra uma issue.

Licença
Este projeto está licenciado sob a MIT License - veja o LICENSE para detalhes.
