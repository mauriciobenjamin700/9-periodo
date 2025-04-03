# "O Desafio do Empréstimo ou Investimento"

Aluno: Mauricio Benjamin da Rocha

**obs**: Inicialmente escrevi os passos e ao final, na seção de **Resposta**, irei apresentar minha resposta para atividade.

## 1. Você está planejando comprar um carro novo e recebeu duas propostas de financiamento

- Ambas as propostas têm o mesmo valor de R$ 20.000,00, mas com diferentes condições.
- Como você decide qual delas escolher? Vamos ver qual delas é mais vantajosa.
- A proposta 1 é de juros compostos (mais comuns em financiamentos bancários).
- A proposta 2 é de juros simples (mais comuns em financiamentos de curto prazo)

## 2. Apresente as condições de financiamento de ambas as propostas (use números realistas)

### Proposta 1 Juros Compostos

- Taxa de juros anual: 12% ao ano
- Prazo: 2 anos

**Como calcular o total a ser pago**:

Usando a fórmula dos juros compostos M=P(1+i)n, onde M é o montante final, P é o valor principal, i é a taxa de juros e n é o número de períodos.

### Proposta 2 Juros Simples

- Taxa de juros anual: 10% ao ano
- Prazo: 2 anos

**Como calcular o total a ser pago**:

Usando a fórmula dos juros simples M=P+Pxixn, onde M é o montante final, P é o valor principal, i é a taxa de juros e n é o número de períodos.

## 3. Siga os Passos

- Calcular o valor total que será pago em cada uma das propostas (usando as fórmulas de juros simples e compostos).
- qual financiamento é mais vantajoso? Quais são as vantagens e desvantagens de cada tipo de juros? Existe alguma estratégia financeira que pode ser usada para "minimizar" os custos no longo prazo?

## 4. Compartilhe suas conclusões com a turma. Pergunte

- **Escolha**: Qual financiamento escolheriam e por quê?
- **Impacto**: Como os juros compostos impactam o montante final?
- **Implicações**: Quais seriam as implicações de escolher um financiamento com juros simples ou compostos para uma compra de longo prazo?

## 5. Após as apresentações, faça uma reflexão sobre o impacto das diferentes taxas de juros e como a Matemática Financeira é crucial para tomar decisões financeiras mais inteligentes. Mostre como a compreensão desses conceitos pode fazer a diferença entre pagar mais ou menos por um financiamento, por exemplo

## Resposta

**Obs**: Em partes envolvendo cálculos, usarei exemplos em script `python` pois em minhas análises financeiras, sempre gosto de automatizar e guardar os exemplos de sucesso.

Todas as respostas estão nas seções a baixo.

### Passo 1: Calcular o valor total a ser pago em cada proposta

**Proposta 1: Juros Compostos**:

- Valor principal: 20.000
- Taxa de juros anual: 12% (0,12)
- Prazo: 2 anos

``` python
principal = 20000
taxa = 0.12
prazo = 2

montante = principal * (1 + taxa) ** prazo # montante = 20000 * (1.12 * 1.12)
print(montante) # montante == 25088
```

Total a ser pago: R$ 25.088,00

**Proposta 2: Juros Simples**:

- Valor principal: 20.000
- Taxa de juros anual: 10% (0,10)
- Prazo: 2 anos

```python
principal = 20000
taxa = 0.10
prazo = 2

juros = principal * taxa * prazo # juros = 20000 * 0.10 * 2 = 4000
montante = principal + juros
print(montante) # montante == 24000
```

Total a ser pago: R$ 24.000,00

### Passo 2: Qual financiamento é mais vantajoso?

Proposta 2 (Juros Simples) é mais vantajosa, pois o total a ser pago é menor (R$ 24.000,00) em comparação com a Proposta 1 (R$ 25.088,00).
A diferença entre as propostas é de R$ 1.088,00.

### Passo 3: Vantagens e desvantagens de cada tipo de juros

- **Juros Compostos**
  - Vantagens:
    - Ideal para investimentos, pois os juros acumulam sobre os juros anteriores.
    - Se você consegue antecipar um certo número de parcelas, acaba por ser uma opção mais interessante.
  - Desvantagens:
    - Para financiamentos, o montante cresce rapidamente, tornando-o mais caro.

- **Juros Simples**
  - Vantagens:
    - Mais previsível e fácil de calcular.
    - O montante cresce de forma linear, sendo mais barato para financiamentos.
  - Desvantagens:
    - Menos vantajoso para investimentos de longo prazo, pois não há acúmulo de juros sobre juros.

**Algumas estrategias que podemos usar:**

- **Negociar taxas de juros menores**: Buscar instituições financeiras que ofereçam taxas mais competitivas.
- **Reduzir o prazo do financiamento**: Quanto menor o prazo, menor será o impacto dos juros compostos.
- **Antecipar parcelas**: Em financiamentos com juros compostos, antecipar parcelas reduz o montante final, pois diminui o tempo de acúmulo de juros.

### Passo 4: Estratégias financeiras para minimizar custos

- **Escolha:**
  - Eu escolheria o financiamento com juros simples (Proposta 2), pois o montante final a ser pago é menor (R$ 24.000,00) em comparação com o financiamento com juros compostos (R$ 25.088,00). A diferença de R$ 1.088,00 representa uma economia significativa, especialmente em um prazo curto de 2 anos. Além disso, os juros simples são mais previsíveis e fáceis de gerenciar.

- **Impacto:**
  - Os juros compostos impactam o montante final de forma exponencial, pois os juros acumulam sobre os juros já calculados. Isso significa que, quanto maior o prazo do financiamento, maior será o crescimento do montante devido. No caso da Proposta 1, mesmo com um prazo curto de 2 anos, o montante final já é consideravelmente maior do que o da Proposta 2.

- **Implicações:**
  - Escolher um financiamento com juros simples é mais vantajoso para compras de curto prazo, pois o crescimento do montante é linear e mais fácil de prever. Por outro lado, optar por um financiamento com juros compostos pode ser mais caro no longo prazo, mas pode ser inevitável em algumas situações, como financiamentos bancários ou prazos mais longos. Nesse caso, é importante planejar o pagamento antecipado de parcelas para reduzir o impacto dos juros acumulados.

Eu particularmente sempre pago a vista, para evitar ao máximo correr o risco dos juros.

### Passo 5: Reflexão

A Matemática Financeira é essencial para tomar decisões financeiras inteligentes. Compreender a diferença entre juros simples e compostos ajuda a evitar gastos desnecessários e a planejar melhor o orçamento. No caso apresentado, escolher a Proposta 2 (juros simples) resulta em uma economia significativa. Além disso, entender o impacto dos juros compostos é crucial para evitar dívidas excessivas em financiamentos de longo prazo.

Uma sugestão vista em sala de aula é sempre organizar os seus gastos atuais e deixar "pago" algum custo para o seu "eu do futuro", assim garantindo uma maior estabilidade em caso de eventos inesperados. Eu gosto particularmente de anotar meus ganhos e custos e fazer alguns scripts para me ajudar a estimar gastos e retornos em possíveis eventos, para ter uma certa margem de erro, em caso de imprevistos.
