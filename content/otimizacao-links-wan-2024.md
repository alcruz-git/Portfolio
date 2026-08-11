title: Otimização de links WAN em 80 locais — 2024
tipo: projeto
area: redes
status: concluido
publish: true
tags: [redes, wan, fortinet, reducao-custos]
data: 2024
stack: [Fortinet]
---

# Otimização de links WAN em 80 locais — 2024

## Contexto
Os locais operavam com links de **2 a 6 Mega**, insuficientes para a demanda
real de banda e performance de cada unidade. A necessidade era clara: mais
banda e melhor performance por local — mas sem elevar o custo total da
operação de links.

## Meu papel
Fui o **responsável principal pelo projeto**, de ponta a ponta:
- Idealizei a melhoria a partir do relacionamento direto com as operadoras,
  papel que eu já exercia como gestor desse relacionamento
- Desenhei o projeto (escopo, dimensionamento de banda por local, priorização)
- Acompanhei toda a implementação em campo, feita pelas equipes das operadoras
  contratadas para a instalação física dos novos links

## Objetivo
Aumentar substancialmente banda e performance dos links em cada local,
mantendo ou reduzindo o custo total da operação — objetivo plenamente atingido.

## O que foi feito
- Redesenho dos contratos de link com as operadoras, substituindo os links
  de 2–6 Mega por links nunca inferiores a 10 Mega
- Dimensionamento por criticidade do local:
  - Maioria dos locais: 20 Mega
  - Alguns locais: 50 Mega
  - Poucos pontos, nos locais mais relevantes: 100 Mega
- Rollout em 80 locais, com mínimo de 2 links por local (mais de 2 nos locais
  operacionalmente mais sensíveis, para redundância)
- Instalação faseada ao longo de vários meses, garantindo continuidade de
  negócio sem interrupção durante os cortes/trocas
- Aproveitamento de recursos já existentes em equipamentos Fortinet instalados
  em projeto anterior, que não estavam sendo usados em todo o potencial

## Decisões técnicas e por quê
- Priorizar o relacionamento direto com as operadoras permitiu negociar
  upgrade de banda mantendo o custo controlado
- Dimensionamento diferenciado por local (10/20/50/100 Mega) em vez de banda
  única para todos: evitou custo excessivo em locais de baixa demanda e
  garantiu banda robusta nos pontos críticos
- Corte dos links feito de forma faseada, local a local, permitindo zero
  interrupção operacional durante toda a migração

## Resultados
| Métrica | Antes | Depois |
|---|---|---|
| Banda por local | 2 a 6 Mega | Mínimo 10 Mega — maioria 20, alguns 50 e 100 Mega |
| Custo mensal com links | Base 100% | Redução de ~60% |
| Throughput/banda efetiva | Base 100% | Aumento de ~80% |
| Locais abrangidos | — | 80 locais (mín. 2 links cada) |
| Continuidade de negócio | — | Sem interrupção durante a migração |
