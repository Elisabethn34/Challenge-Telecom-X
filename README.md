Relatório Final – Análise de Evasão de Clientes (Churn)
Este projeto tem como objetivo analisar o problema de evasão de clientes (churn) em uma empresa de telecomunicações. Através da análise exploratória dos dados, buscamos compreender o comportamento dos clientes que cancelam os serviços e identificar padrões que ajudem a reduzir a taxa de cancelamento.

A retenção de clientes é um fator estratégico para qualquer empresa, e entender os fatores que levam ao churn permite que ações preventivas sejam tomadas.

Limpeza e Tratamento de Dados
As seguintes etapas foram realizadas:

Importação de dados no formato JSON, com estrutura aninhada.
Normalização das tabelas internas (cliente, plano, internet, cobrança).
Padronização dos nomes das colunas para snake_case.
Conversão de colunas como charges.total de texto para valor numérico (float), tratando valores nulos.
Criação da coluna contas_diarias dividindo charges.monthly por 30.
Substituição dos valores de churn: Yes → Cancelou, No → Permaneceu.
Análise Exploratória de Dados (EDA)
Distribuição de Evasão (Churn)
A maioria dos clientes permaneceu.
Cerca de 26,6% dos clientes cancelaram o serviço.
Gráfico de pizza com rótulo percentual e número absoluto foi gerado para representar a proporção.

Churn por Variáveis Categóricas
Foi analisada a distribuição de cancelamentos com base em variáveis como:

Tipo de contrato (contract)

Contratos mensais lideram em evasão.
Forma de pagamento (paymentmethod)

Métodos automáticos têm menor taxa de churn.
Outras variáveis categóricas analisadas:
gender, partner, internetservice, multiplelines

Gráficos de barras foram usados para cada variável, com percentuais visuais.

Churn por Variáveis Numéricas
Utilizamos boxplots para comparar a distribuição de:

tenure (tempo de contrato)

Clientes com pouco tempo de casa tendem a cancelar mais.
charges.monthly (gasto mensal)

Clientes com gasto mensal mais alto costumam permanecer.
charges.total (gasto total)

Clientes com maior histórico de gastos têm menor taxa de churn.
Também foi calculada a média, mediana e desvio padrão dessas variáveis separadas por grupo de churn.

Principais Conclusões
Contratos mensais têm alta taxa de evasão.
Tempo de contrato curto é um forte indicador de churn.
Menor gasto total ou mensal está associado a maior cancelamento.
Clientes que pagam com métodos automáticos permanecem mais.
Recomendações
Oferecer vantagens para planos anuais, como descontos e benefícios.
Implementar ações de retenção precoce (ex: apoio proativo nos primeiros meses).
Estimular formas de pagamento automáticas.
Criar campanhas para usuários de baixo gasto total.
Monitorar clientes com menor tempo de contrato para ações direcionadas.
Conclusão
Através dessa análise, foi possível entender os perfis com maior risco de evasão e propor estratégias concretas para reduzir a perda de clientes. A análise baseada em dados torna as decisões mais inteligentes e eficazes.

