# Sistema de Gerenciamento de Missões Espaciais🚀

Este é um sistema em Python para gerenciar astronautas, equipes, missões espaciais e espaçonaves. Utilizando o **SQLAlchemy** e um banco de dados SQLite, o projeto permite realizar diversas operações de CRUD (Criar, Ler, Atualizar, Deletar) para controlar astronautas, equipes, missões e espaçonaves, além de permitir a monitorização do andamento das missões e o gerenciamento de problemas com as espaçonaves.

## Funcionalidades

O sistema oferece as seguintes funcionalidades:

### 1. Gerenciamento de Astronautas👨‍🚀
- **Adicionar astronauta**: Cadastra um novo astronauta com nome e especialidades.
- **Remover astronauta**: Remove um astronauta do banco de dados.
- **Consultar astronautas**: Exibe todos os astronautas cadastrados, mostrando seu nome e especialidades.
- **Atualizar astronauta**: Permite atualizar o nome e as especialidades de um astronauta já registrado.

### 2. Gerenciamento de Equipes👥
- **Criar equipe**: Cria uma nova equipe, permitindo adicionar astronautas a ela.
- **Listar equipes**: Exibe todas as equipes cadastradas no sistema, incluindo os astronautas que fazem parte de cada uma.

### 3. Gerenciamento de Missões🌙
- **Criar missão**: Cria uma nova missão e a associa a uma equipe.
- **Consultar missões**: Exibe todas as missões cadastradas, incluindo informações sobre sua data de início, data de fim e status (ativa ou finalizada).
- **Iniciar missão**: Marca uma missão como iniciada e registra sua data de início.
- **Finalizar missão**: Marca uma missão como finalizada e registra sua data de término.
- **Monitorar missão**: Exibe informações detalhadas sobre uma missão ativa, incluindo a equipe associada e a espaçonave, caso já tenha sido lançada.

### 4. Gerenciamento de Espaçonaves🚀
- **Adicionar espaçonave**: Registra uma nova espaçonave com informações sobre seu modelo e capacidade de carga.
- **Lançar espaçonave**: Associa uma espaçonave a uma missão ativa e registra o lançamento.
- **Reportar problema**: Permite registrar problemas relacionados à capacidade de carga de uma espaçonave associada a uma missão ativa.

## Tecnologias Utilizadas

- **Python**: Linguagem de programação utilizada para implementar o sistema.
- **SQLAlchemy**: ORM (Object-Relational Mapping) usado para manipular o banco de dados SQLite.
- **SQLite**: Banco de dados utilizado para armazenar as informações do sistema.
- **Datetime**: Módulo utilizado para gerenciar as datas de lançamento e finalização das missões.

## Estrutura do Banco de Dados

O sistema utiliza as seguintes tabelas no banco de dados:

1. **Astronautas**: Armazena informações sobre os astronautas, como nome e especialidades.
2. **Equipes**: Armazena informações sobre as equipes, associando astronautas a equipes.
3. **Missões**: Armazena informações sobre as missões espaciais, como nome, datas de início e fim, e status.
4. **Espaçonaves**: Armazena informações sobre as espaçonaves, como modelo, capacidade de carga e status de problemas.
5. **Centro de Controle**: Armazena informações sobre os centros de controle das missões.

## Como Usar

1. **Instalar as dependências**:
   
   - Para rodar o projeto, você precisa do Python 3.x e das bibliotecas SQLAlchemy. 
   - Crie e ative um ambiente virtual (opcional):
     ```bash
     python -m venv venv
     source venv/bin/activate  # No Windows use venv\Scripts\activate
     ```
   - Instale as dependências:
     ```bash
     pip install sqlalchemy
     ```

2. **Executar o código**:
   
   Após configurar o ambiente, basta rodar o script Python:
   ```bash
   python nome_do_script.py
