# Sistema de Gerenciamento de Eventos

## Visão Geral
Este projeto é um Sistema de Gerenciamento de Eventos projetado para lidar com eventos, participantes e check-ins. Ele fornece funcionalidades para registrar eventos, gerenciar participantes e realizar check-ins para os participantes. O sistema é implementado usando Python com Flask para o backend e SQLAlchemy para o gerenciamento do banco de dados.

## Estrutura do Projeto

### Modelos
- **Participantes**: Representa informações sobre os participantes do evento.
- **Check-ins**: Registra os check-ins feitos pelos participantes.
- **Eventos**: Contém detalhes sobre os eventos.

### Repositórios
- **Repositório de Participantes**: Lida com operações relacionadas a participantes no banco de dados.
- **Repositório de Check-in**: Gerencia operações de check-in no banco de dados.
- **Repositório de Eventos**: Responsável por operações relacionadas a eventos no banco de dados.

### Manipuladores
- **Manipulador de Participantes**: Lida com solicitações HTTP relacionadas a participantes, como registro de participantes, recuperação de crachás de participantes e busca de participantes em um evento.
- **Manipulador de Check-in**: Gerencia solicitações HTTP para operações de check-in.
- **Manipulador de Eventos**: Lida com solicitações HTTP relacionadas a eventos, como registro de eventos e recuperação por ID.

### Rotas
- **Rotas de Participantes**: Contém endpoints para operações relacionadas a participantes.
- **Rotas de Check-in**: Inclui endpoints para funcionalidades de check-in.
- **Rotas de Eventos**: Contém endpoints para operações relacionadas a eventos.

### Erros
- **Tipos de Erro**: Define tipos de erros personalizados, como HttpConflictError e HttpNotFoundError.
- **Manipulador de Erros**: Gerencia o tratamento de erros e retorna respostas HTTP apropriadas.

### Utilitários
- **Tipos HTTP**: Define classes de solicitação e resposta HTTP.

### Servidor
- **Servidor**: Inicializa e configura a aplicação Flask.

## Configuração e Execução
1. Clonar o repositório.
2. Navegar até o diretório do projeto.
3. Instalar as dependências usando `pip install -r requirements.txt`.
4. Garantir que a conexão com o banco de dados esteja configurada corretamente.
5. Executar o servidor Flask usando `python src/models/repository/events_repository.py`.

## Testes
- Arquivos de teste são fornecidos para os repositórios para garantir que as operações do banco de dados funcionem conforme o esperado.
- Use `pytest` para executar os testes.

## Dependências
- Flask: Um framework leve de aplicação web WSGI.
- SQLAlchemy: Um toolkit SQL e uma biblioteca de Mapeamento Objeto-Relacional (ORM) para Python.

