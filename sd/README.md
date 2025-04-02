# Sistemas Distribuídos

- Disponibilidade
- Tempo de resposta < X
- Confiabilidade
- Tolerância a falha
- Escalabilidade

## Definições

É um **conjunto de computadores independentes** que se apresenta a seus usuários como um sistema **único e coerente**.

## Metas

- Escalabilidade e Distribuição Global
- Hardware de Alto Desempenho
- Redes de Alta Velocidade
- Computação em Nuvem e Virtualização
- Segurança e Privacidade
- Inteligência Artificial e Automação

### ATAE

- ACESSO (A) - Oferecer fácil acesso a seus recursos
- TRANSPARÊNCIA (T) - Oferecer transparência
- ABERTO (A) Deve ser aberto
- ESCALÁVEL (E) Deve ser escalável

## Middleware

- Client ->  Request -> Middleware -> Server
- Server -> Middleware -> Request - Client

- App - Middleware -> SO

## Tipos de Computação Distribuídos

- Sistemas de computação distribuída
- Sistemas de informação distribuída
- Sistemas de 

### Tipos de

- Cluster - Agrupamento em Nodes por switch organizados por um node Master, acessados por usuários via o master.
- Grid - Elementos dispersos geograficamente na rede.
- Cloud - Virtualizada e Gerenciada por servidores

## Computação em Nuvem

### Características Essenciais

- Amplo de Acesso (Usuário)
- Utilidade (Usuário)
- Pooling de recursos (Usuário e Servidor)
- Self-service (Usuário)
- Serviço monitorado (Servidor)
- Elasticidade (Servidor)

## Arquitetura

Quais componentes e como se relacionam.

### O que é

- Organização
- Planejamento
- Design

### Software

- Padrão de projeto
- Refatoração
- Modularidade

### Oque é um componente?

- Interface clara (Como oferecer e consumir serviços)

### Estilo Arquitetônico x Arquitetura de Sistema

- Estilo Arquitetônico (Relacionado ao software)
- Arquitetura de Sistema (Relacionado ao hardware/Topologia)

### Quanto estilos em SDs

- Arquiteturas em camadas
- Arquiteturas baseadas em objetos
- Arquiteturas centradas em dados
- Arquitetura baseadas em eventos
- Arquitetura de microsserviços

#### Arquitetura em camadas

- Cada camada fala somente com as camadas próximas
- Segurança e validação em cada camada

- **Vantagens**

- Separação calara de responsabilidades
- Fácil de modificar ou substituir camadas individuais

- **Desvantagens**

- Pode ter impacto no desempenho (Vários níveis de chamada)
- Interação entre camadas não adjacentes é difícil ou proibida

#### Arquiteturas baseadas em objetos

- **Vantagens**

- Alta reutilização de código
- Facilidade de modelagem (Orientação a objetos)

- **Desvantagens**

- Pode gerar forte acoplamento entre muitos objetos
- Difícil de escalar em sistemas muito grandes

#### Arquiteturas centradas em dados

Componentes publicam dados enquanto outros componentes buscam dados

- **Vantagens**

- Compartilhamento simples de dados
- Boa para integrar sistemas heterogêneos

- **Desvantagens**

- Escalabilidade
- Sobrecarga em consultas, para escrita por exemplo

#### Arquitetura baseadas em eventos

### Arquiteturas de sistemas

#### Arquiteturas centralizadas

Vantagens

- Simplicidade
- Controle total
- Boa performance em sistemas pequenos

- Desvantagens

- Gargalos

#### Arquitetura descentralizada

#### Arquitetura hibrida

## Review

- escalabilidade
  - vertical: recursos computacionais (RAM, CPU)
  - Horizontal: mais nos
- distribuição
  - vertical: Funções diferentes ( sistemas diferentes )
  - horizontal: Funções iguais ( replicas executando a mesma função)

### P2P

- Centralização
- Desconexão
- Interação simétrica
- Fácil entrada, fácil Saida

#### Arquitetura P2P Estruturada

- guarda chave e valores
- Usada tabela hash desatribuída para guardar todos os nos
- cada no conhece apenas o no anterior e o proximo, mas pode ser possível ir para outros nos distantes usando a tabela hash

#### Arquitetura P2P N Estruturada

- Cada no, guarda uma lista de vizinhos, de forma aleatória.
- Tudo depende do algoritmo
- Busca por inundação

