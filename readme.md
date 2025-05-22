# Funcionamento do models, controllers e endpoints no projeto

O funcionamento do models interage diretamente com o banco de dados, realizando consultas a ele e o controllers realiza o intermédio entre a camada model e a view, agindo como uma espécie de ponte entre ambos, transferindo dados por meio do processo de requisição e resposta. Já os endpoints consistem em URLs que direcionam a APIs, de modo que sejam realizadas requisições. No contexto desta atividade, verifica-se a presença de endpoints nos arquivos presentes na pasta routes, uma vez que neles há os caminhos para as requisições serem realizadas, especialmente no escopo de aluno, professor e curso.


## Requisitos

- Node.js
- PostgreSQL

## Instalação

1. **Clonar o repositório:**

```bash
   git clone https://github.com/luanalima77/aulaSemana4Modulo2Computacao.git
   cd aulaSemana4Modulo2Computacao
```

2. **Instalar as dependências:**
    
```bash
npm install
```
    
3. **Configurar o arquivo `.env`:**
    
Renomeie o arquivo `.env.example` para `.env` e configure as variáveis de ambiente necessárias, como as configurações do banco de dados PostgreSQL.
    

Configuração do Banco de Dados
------------------------------

1. **Criar banco de dados:**
    
    Crie um banco de dados PostgreSQL com o nome especificado no seu arquivo `.env`.
    
2. **Executar o script SQL de inicialização:**
    
```bash
npm run init-db
```
    
Funcionalidades
---------------

* **Padrão MVC:** Estrutura organizada em Model, View e Controller.
* **PostgreSQL:** Banco de dados relacional utilizado para persistência dos dados.

Scripts Disponíveis
-------------------

* `npm start`: Inicia o servidor Node.js.
* `npm run dev`: Inicia o servidor com `nodemon`, reiniciando automaticamente após alterações no código.
* `npm run test`: Executa os testes automatizados.
* `npm run test:coverage`: Executa os testes e gera um relatório de cobertura de código.

Estrutura de Diretórios
-----------------------

* **`config/`**: Configurações do banco de dados e outras configurações do projeto.
* **`controllers/`**: Controladores da aplicação (lógica de negócio).
* **`models/`**: Modelos da aplicação (definições de dados e interações com o banco de dados).
* **`routes/`**: Rotas da aplicação.
* **`tests/`**: Testes automatizados.
* **`views/`**: Views da aplicação (se aplicável).
