# post_message_websocket
- Este projeto contém dos serviços que postam mensagens para o websocket. 
- Comandos para subir a aplicação:
-- docker network create app_network
-- docker-compose up -d

- 1° serviço: API PYTHON RESTFULL FAST API: Ao chamar o endpoint: http://localhost:8082/send_message e enviar uma mensagem: 
{
	"message": {
		"Teste": "Teste de envio de mensagens para o websocket"
	}
}
A mesma será consumida pelo websocket.
- 2° serviço sobe automaticamente junto ao docker e realiza a postagem de mensagens a cada 5 segundos.
