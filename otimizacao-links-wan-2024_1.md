---
title: Otimização de links WAN em 80 locais — 2024
tipo: projeto
area: redes
status: em-andamento
publish: false
tags: [redes, wan, fortinet, reducao-custos]
data: 2024
stack: [Fortinet]
---

# Otimização de links WAN em 80 locais — 2024

## Contexto
Os locais operavam com links de **2 a 6 Mega**, insuficientes para a demanda
real de banda e performance de cada unidade. A necessidade era clara: mais
banda e melhor performance por local — mas sem elevar o custo total da
operação de links, que já era um item relevante do orçamento de TI.

## Meu papel
Fui o **responsável principal pelo projeto**, de ponta a ponta:
- Idealizei a melhoria a partir do relacionamento direto com as operadoras,
  papel que eu já exercia como **gestor do relacionamento com operadoras**
- Desenhei o projeto (escopo, dimensionamento de banda por local, priorização)
- Acompanhei toda a implementação em campo, feita pelas equipes das operadoras
  contratadas para a instalação física dos novos links

## Objetivo
Aumentar substancialmente banda e performance dos links em cada local,
**mantendo ou reduzindo o custo total** da operação — objetivo **plenamente
atingido**.

## O que foi feito
- Renegociação/redesenho dos contratos de link com as operadoras, substituindo
  os links de 2–6 Mega por links **nunca inferiores a 10 Mega**
- Dimensionamento por criticidade do local:
  - Maioria dos locais: **20 Mega**
  - Alguns locais: **50 Mega**
  - Poucos pontos, nos locais mais relevantes/críticos: **100 Mega**
- Rollout em 80 locais, com mínimo de 2 links por local (mais de 2 nos locais
  operacionalmente mais sensíveis, para redundância)
- Instalação faseada ao longo de vários meses, coordenada para garantir
  **continuidade de negócio sem interrupção** durante os cortes/trocas
- Aproveitamento de recursos já existentes nos equipamentos **Fortinet**
  instalados em projeto anterior, que não estavam sendo usados em todo o
  potencial (recurso explorado para extrair melhor performance dos novos links)

## Decisões técnicas e por quê
- Priorizar o relacionamento direto com as operadoras (em vez de licitação
  aberta ampla) permitiu negociar upgrade de banda mantendo o custo controlado
  — decisão apoiada na posição de gestor desse relacionamento
- Dimensionamento diferenciado por local (10/20/50/100 Mega) em vez de banda
  única para todos: evitou pagar de mais em locais de baixa demanda e garantiu
  banda robusta nos pontos críticos
- Corte dos links feito de forma faseada/local a local, não em massa, o que
  permitiu zero interrupção operacional durante toda a migração

## Resultados / métricas
| Métrica | Antes | Depois |
|---|---|---|
| Banda por local | 2 a 6 Mega | Mínimo 10 Mega — maioria 20 Mega, alguns 50 e 100 Mega |
| Custo mensal com links | Base 100% | **Redução de ~60%** |
| Throughput/banda efetiva | Base 100% | **Aumento de ~80%** |
| Locais abrangidos | — | 80 locais (mín. 2 links cada) |
| Continuidade de negócio | — | Sem interrupção durante a migração |

## Lições aprendidas
[A PREENCHER, se quiser incluir: maior desafio de coordenação com as
operadoras, algo que faria diferente hoje, como validou que não houve
interrupção durante os cortes]

## Evidências (sanitizadas)
[A PREENCHER antes de publicar: diagrama de banda por local (antes/depois),
cronograma de rollout dos 80 locais, print de dashboard Fortinet mostrando
utilização — sempre sem nomes reais de operadoras, clientes ou sites]

---
### Nota para publicação no portfólio
Antes de mover para `04-Portfolio/`:
1. Confirmar/remover os campos `[A PREENCHER]`
2. Verificar se "80 locais" e os percentuais podem ser divulgados publicamente
   (ou se precisam ser generalizados, ex: "dezenas de locais")
3. Remover qualquer nome de cliente, operadora ou identificador de site
4. Só então trocar `publish: false` → `publish: true`
