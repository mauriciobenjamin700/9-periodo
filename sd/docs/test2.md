# SO: Threads, Processos e Programa

- Privilégios
- Isolamento
- Segurança
- Eficiência

Distribuição de tarefas entre o mestre e os escravos

## Balanceamento de Carga

- Random
- Sequential (Round Robin)
- Utilization Level

## Virtualização

Inserir mais camadas de aplicação em cima de aplicação que já está em cima do hardware

- Imagens: Empacotamento de maquinas virtuais de forma estática
- Interfaces: Cada camada é uma interface que permite a comunicação desde aplicação, biblioteca, sistema operacional e hardware. Existem outras mas estas são as mais comuns.

Virtualização consiste em imitar camadas do sistema.

### VM

### Containers

Os containers garantem código, dependências e sistemas operacionais.

Benefícios

- Portabilidade
- Isolamento
- Eficiência
- Escalabilidade

## Classificação de Falhas

### Falhas de comunicação

- Confiabilidade
- Tempo

### Falhas de Processamento

- Interrupções inesperadas
- Erros de execução
- Problemas de concorrência
- Mau gerenciamento de recursos

### Falhas Temporais

- Desalinhamento de relógios
- Atrasos de execução
- Time-outs indevidos (Network Time Protocol -> NTP)

### Falhas Omissivas e Bizantinas

- Falhas Omissivas (Não houve resposta)
- Falhas Bizantinas (Resposta errada)

### Falhas Humanas e Operacionais

- Erro de configuração
- Atualizações mal testadas

- Interrupções operacionais
- Permissões erradas

## Detecção de Falhas

### Heartbeat

- De tempos em tempos, o escravo avisa ao mestre que está vivo.
- Se o sinal não for recebido dentro de um intervalo, o nó será considerado inativo.
- Pode ser unidirecional ou bidirecional.

Vantagens:

- Monitoramento
- Detectando Falhas
- Acionando Ações de Recuperação
- Balanceamento de Carga

### TImeOuts e Suposições de Falha

- Timeout (Requisições abandonadas)
- Pode causar falsos positivos
- O tempo ideal depende do contexto

### Watchdog TImers

- Processo ou hardware que monitora outro processo.
- Se o processo monitorado travar ou deixar de enviar sinais. O watchdog reinicia ou gera alarme.

### Ferramentas de Monitoramento

- Prometheus
- Grafana
- ELK Stack

## Estratégias de Tolerância

### Redundância (nós)

- Redundância hot standby
- Redundância cold standby
- Redundância warm standby

### Failover Automático

Gatilho que irá gerar uma ação, caso algum nó caia.

- Mecanismo que detecta falhas e redireciona requests ou migra apps para outro nó

### Reexecução de tarefas

## Estratégias de Recuperação

- Checkpoint e Rollback
- Exponential Backoff
- Jitter Backoff
- Linear Backoff
- Logs
