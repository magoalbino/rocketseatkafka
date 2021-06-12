# Micro-serviço com Node.js

- Utilizando kafka;
- Utilizando Node;

## Aplicações

- API principal (Station);
- Geração de certificado;

## Fluxo

- API principal envia uma mensagem pro serviço de certificado para gerar o certificado;
- Micro-serviço de certificado devolve uma resposta (síncrona/assíncrona)

Se conseguir síncrona/assíncrona:
- Receber uma resposta assíncrona de quando o e-mail com o certificado foi enviado;

## O que sabemos?

- REST (latência)
- Redis / RabbitMQ / **Kafka** (nubank, uber, paypal, netflix);

## Conclusão

- Utilizamos um simulador de requisição (extensão do chrome ou postman) para localhost:3333
- Conseguimos observar a mensagem enviada pela requisição no serviço que gera o certificado fictício, e a resposta recebida por ele no serviço API

- 'yarn dev' na api e na certification
- docker-compose up -d na raíz
