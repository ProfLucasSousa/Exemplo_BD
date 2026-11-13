# Exemplo de Banco de Dados com PHP

Projeto didático de PHP e MySQL baseado em um esquema de Recursos Humanos. O exemplo cria tabelas relacionadas e oferece telas para cadastrar e listar regiões e países.

## Conteúdo

Os arquivos do projeto estão diretamente na raiz.

- `RH.sql`: cria e popula o banco `RH`.
- `conexao.php`: conexão com o MySQL.
- `cadastrar_regiao.php` e `cadastrar_pais.php`: formulários de cadastro.
- `listar_regiao.php` e `listar_pais.php`: consultas e listagens.
- `classesFormulario/`: classes PHP para montar elementos de formulário.

## Como executar

1. Importe o banco:

```bash
mysql -u root -p < RH.sql
```

2. Ajuste usuário, senha, host e banco em `conexao.php`.
3. Inicie o servidor local:

```bash
php -S localhost:8000
```

4. Acesse `http://localhost:8000`.

## Modelo de dados

O script SQL trabalha com regiões, países, localizações, funções, departamentos, funcionários e histórico de funções, conectados por chaves estrangeiras.

Projeto voltado a estudo. Para uso real, revise validação, tratamento de erros e consultas ao banco.
