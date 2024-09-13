# FastAPI WebSocket Application with JWT Authentication

## Descrição

Este projeto é uma aplicação WebSocket utilizando FastAPI com autenticação JWT. A aplicação permite que os usuários se autentiquem, conectem-se a diferentes "salas" (rooms) via WebSocket e enviem mensagens que são armazenadas e retransmitidas para todos os clientes conectados na mesma sala. Além disso, a aplicação permite que os usuários vejam o histórico de mensagens de uma sala mesmo após se reconectar.

## Funcionalidades

- Autenticação de usuários com JWT.
- Conexão a diferentes salas via WebSocket.
- Armazenamento e recuperação de mensagens por sala, com timestamps.
- Broadcast de mensagens para todos os clientes conectados na mesma sala.
- Manutenção do histórico de mensagens de uma sala, mesmo após desconexões e reconexões.

## Instalação

Antes de começar, certifique-se de ter instalado o Python 3.8 ou superior em seu computador.

### criar ambiente virtual
1.python -m venv venv  
2.source venv/bin/activate  
No Windows, use: venv\Scripts\activate

### instalar as dependências
3.pip install -r requirements.txt

### iniciar o servidor
uvicorn main:app --host 0.0.0.0 --port 8000 --reload


