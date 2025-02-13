# Evolution API

Este repositório contém a configuração para executar a Evolution API via Docker Compose.

## Como Usar

1. **Configurar Variáveis de Ambiente**
   
   - Renomeie o arquivo `.env.exemple` para `.env` e ajuste os valores conforme necessário.

2. **Criar a Rede Externa (se necessário)**

   Certifique-se de que a rede externa `n8n-flow_intnet` existe:
   
   ```bash
   docker network create n8n-flow_intnet
   ```

3. **Iniciar a Aplicação**

   Inicie os serviços:
   
   ```bash
   docker-compose up -d
   ```

   A API estará disponível na porta **8080**.

## Parar a Aplicação

Para interromper os containers:

```bash
docker-compose down
```

