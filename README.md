# go-expert-challenge-auction

## Como Iniciar o Projeto

1. **Subir o MongoDB e a Aplicação**
   Execute o seguinte comando para iniciar os serviços:
   ```bash
   docker compose up -d
   ```

2. **Configuração de Variáveis de Ambiente**
   O arquivo `.env` contém as variáveis de ambiente que controlam o comportamento do sistema:
   
   - `AUCTION_EXPIRED`: Define o tempo de expiração de um leilão. Valor padrão: **20 segundos**.
   - `FETCH_EXPIRED_INTERVAL`: Controla o intervalo de verificação para identificar leilões expirados. Valor padrão: **10 segundos**.

## Como Executar os Testes

Execute os testes utilizando o seguinte comando:
```bash
docker compose exec app go test ./internal/infra/database/auction -v
```
