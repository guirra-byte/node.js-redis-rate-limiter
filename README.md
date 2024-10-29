# **`Advanced Rate Limiter with Node.js and Redis`**

> [!CAUTION]
> **`Classificação de dificuldade do desafio`**: **Alta**
> 
Resolução do desafio de implementar um **Rate Limiter Avançado**. Deve ser desenvolvido em **Node.js** com integração ao **Redis** para armazenamento de dados de limite e alta escalabilidade. O objetivo é implementar uma solução robusta para o controle de requisições, suportando múltiplas estratégias de limitação de acesso e adaptável a diferentes níveis de tráfego, endpoints e configurações.

## Funcionalidades

- **Múltiplas Estratégias de Rate Limiting**:
  - **Fixed Window**: Controle de limite fixo por janela de tempo.
  - **Sliding Window**: Controle contínuo e adaptável.
  - **Token Bucket**: Regulação de requisições por meio de tokens.

- **Persistência com Redis**:
  - Uso de Redis para armazenamento de contadores, timestamps e tokens.
  - Suporte a clusters Redis para distribuição e escalabilidade.

- **Configurações Customizáveis**:
  - Limitação de requisições por IP ou usuário.
  - Configuração por endpoint para maior controle e flexibilidade.
  - Arquivo de configuração JSON para ajustes dinâmicos.

- **Monitoramento e Feedback**:
  - Cabeçalhos detalhados (`X-RateLimit-Limit`, `X-RateLimit-Remaining`, `Retry-After`) para o cliente.
  - Endpoint de métricas em tempo real com informações sobre limites de requisição, requisições bloqueadas e permitidas.

## Tecnologias Utilizadas

- **Node.js** - Backend para implementação do rate limiter.
- **Redis** - Armazenamento de dados de limite e suporte a alta escalabilidade.
- **Docker** - Conteinerização para fácil deploy e escalabilidade.
- **Express** - Framework Node.js para criação do servidor e endpoints.
