# Tarefa 02 - Conexão Banco de Dados com ODBC e ORM

Atividade de acesso a banco de dados em **TypeScript**, usando dois métodos contra o mesmo banco PosgreSQL:
1. Acesso por **driver direto** (biblioteca pg).
2. Acesso via código orientado a objetos.

Toda a infraestrutura (PgAdmin e aplicação TypeScript) sob via Docker Compose.

# Estrutura das pastas e arquivos
```
- database/
  - 20252/
    - tarefas/
      - vitoria31032003/
        - docker-compose.yml
        - odbc.ts
        - orm.ts
        - package.json
        - package-lock.json
        - tarefa-orm.md
```
# Links dos arquivos
Configuração do docker compose: (https://github.com/vitoria31032003/eng-software-2/blob/tarefa01/database/20252/tarefas/vitoria31032003/docker-compose.yml)

ODBC: (https://github.com/vitoria31032003/bsi-tasks/blob/tarefa01/database/20252/tarefas/vitoria31032003/odbc.ts)

ORM: (https://github.com/vitoria31032003/bsi-tasks/blob/tarefa01/database/20252/tarefas/vitoria31032003/orm.ts)

Dependências internas: (https://github.com/vitoria31032003/bsi-tasks/blob/tarefa01/database/20252/tarefas/vitoria31032003/package-lock.json)

Dependências do projeto: (https://github.com/vitoria31032003/bsi-tasks/blob/tarefa01/database/20252/tarefas/vitoria31032003/package.json)

**ODBC:** É uma API padrão desenvolvido pela  Microsoft e Simba Technologies no início dos anos 1990, torna-se uma base para a Interface de Nível de Chamada padronizada pelo SQL Access Group nos campos Unix e mainframe. O ODBC criou várias funcionalidades que foram removidas como parte do esforço de CLI, tornasse um ODBC completo para essa essas plataformas, sendo um padrão de fato consideravelmente mais conhecido que o CLI.

Em TypeScripy, o método clássico para usar ODBC é importado a biblioteca **odbc**, que implementa as operações básicas do banco. O fluxo é sempre o mesmo de execução: importa a biblioteca, abrir a conexão com banco, driver conecta no banco PosgreSQL, executa comandos, exbie através no console e fecha a conexão. Tudo isso feito em SQL.

**TypeORM** É um ORM que permitir aos desenvolvedores trabalhem utizando bancos de dados relacionais tendo uma abordagem orientada a objetos, o TypeORM foi escrito em TypeScripy e projetado para ser usado com Node.js. Ele suporta os principais bancos de dados, incluindo MySQL, PostgreSQL, MariaDB, SQLite, e até mesmo Microsoft SQL Server. 

Com TypeORM podemos definir entidades e relacionamentos diretamente no código em TypeScript, possibilitando uma integração perfeita entre a lógica da aplicação e o banco de dados. Também oferece suporte a migrações de banco de dados, permitindo que mantenha o esquema do banco de dados sincronizado com o código de aplicação.
