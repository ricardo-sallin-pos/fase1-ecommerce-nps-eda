# Previsão e Análise de NPS em E-commerce

## Visão Geral

O cenário analisado mostra um aumento no volume de vendas acompanhado por uma queda relevante no NPS.

O principal ponto é que a coleta do NPS acontece apenas após toda a jornada do cliente (compra, entrega e pós-venda), o que compromete a previsibilidade e impede ações antecipadas.

O objetivo deste trabalho é entender quais variáveis impactam a experiência do cliente e gerar direcionamentos para atuação preventiva.

---

## Problema de Negócio

* Crescimento de vendas com redução da satisfação
* NPS médio em torno de **-64**, indicando cenário crítico
* Baixa capacidade de antecipar insatisfações

Impacto:

* Aumento de churn em um ambiente com baixa barreira de troca
* Perda de fidelização e receita

---

## Contexto

No e-commerce, o cliente tem facilidade para comparar preços e migrar para concorrentes.

Isso torna o NPS um indicador central para:

* Fidelização
* Recompra
* Sustentação da receita

As áreas diretamente impactadas são:

* Logística
* Atendimento
* Produto e catálogo
* Estratégia de pricing

---

## Principais Achados da Análise

### 1. Problemas operacionais são predominantes

A análise exploratória evidenciou:

* Alto volume de pedidos com atraso
* Pedidos com múltiplas reclamações
* Necessidade de múltiplos contatos com suporte
* Tempo elevado de resolução
* Entregas com mais de uma tentativa

Esse conjunto de fatores explica o nível crítico de NPS observado.

---

### 2. Entrega e pós-venda concentram o impacto

A análise de correlação, separando a jornada em três etapas, mostrou:

**Compra**

* Baixa correlação com o NPS

**Entrega**

* Dias de atraso com forte relação negativa

**Pós-venda**

* Reclamações, contatos e tempo de resolução com impacto direto no NPS

---

### 3. Pequenas variações geram grandes impactos

A análise de contingência mostrou mudanças abruptas no comportamento:

* 1 reclamação → ~3% detratores
* 2 reclamações → ~57% detratores

Indicação clara de que a experiência degrada rapidamente com acúmulo de problemas.

---

## Variáveis Identificadas no Modelo

A regressão múltipla, com controle de multicolinearidade via VIF, indicou como principais variáveis:

* Atraso na entrega
* Quantidade de reclamações
* Tempo de resolução
* Número de contatos com suporte

---

## Impacto das Variáveis no NPS

* Atraso na entrega: **-0,95 por dia**
* Reclamações: **-0,4 por ocorrência**
* Contatos com suporte: **-0,3 por interação**

Cada dia de atraso aumenta significativamente o risco de transformar um promotor em neutro ou detrator.

---

## Conclusão

A queda no NPS é explicada principalmente por falhas na entrega e no pós-venda.

O maior potencial de melhoria está em:

* reduzir atrasos
* diminuir quantidade de contatos

Pequenas melhorias nesses pontos têm impacto direto e relevante na satisfação do cliente.
