---
title: Atualização do ambiente de firewall — Grupo Belarmino (2023)
tipo: projeto
area: redes
status: concluido
publish: true
tags: [redes, seguranca, firewall, fortinet, sonicwall]
data: 2023
empresa: Grupo Belarmino
stack: [Fortinet, FortiManager, FortiAnalyzer, HA]
---

# Atualização do ambiente de firewall — Grupo Belarmino (2023)

## Contexto
Projeto extenso de atualização do ambiente de firewall do Grupo Belarmino,
substituindo aproximadamente 90 firewalls **Sonicwall** por firewalls
**Fortinet**, um por localidade, distribuídos entre a matriz e as diversas
localidades da empresa.

## Meu papel
Liderei e coordenei o projeto do lado do cliente, conduzindo toda a
implementação e parte das configurações, com apoio de uma empresa
especializada terceira, responsável pela estruturação do projeto e pelo
acompanhamento com especialistas.

## Objetivo
Modernizar o ambiente de segurança de rede substituindo o parque Sonicwall
por Fortinet, sem interromper a operação das aproximadamente 90 localidades
durante a migração.

## O que foi feito
- Substituição de ~90 firewalls Sonicwall por Fortinet (FortiGate), um por
  localidade
- Instalação em **alta disponibilidade (HA)** na matriz
- Cada localidade contava com dois links (um principal de produção e um
  secundário) — a migração aproveitou essa redundância: o novo firewall
  entrava primeiro pelo link secundário, não produtivo, e só depois assumia
  o link principal
- Rollout faseado, localidade a localidade, com agendamento prévio para
  minimizar risco de indisponibilidade
- Gerenciamento centralizado via **FortiManager**
- Definição e filtragem de regras de firewall
- Coleta e análise de dados via **FortiAnalyzer**

## Decisões técnicas e por quê
- A entrada gradual pelo link secundário antes do principal permitiu validar
  cada novo firewall em produção real, sem expor o link principal a risco
  até a confiança no ambiente estar estabelecida
- O rollout localidade a localidade, em vez de uma virada única, reduziu a
  superfície de risco de qualquer interrupção durante a troca de ~90 pontos
- Gerenciamento centralizado (FortiManager) e coleta de dados (FortiAnalyzer)
  desde o início garantiram visibilidade e padronização das regras em todas
  as localidades

## Resultados
- ~90 localidades migradas de Sonicwall para Fortinet, sem interrupção da
  operação
- Matriz operando em alta disponibilidade (HA)
- Ambiente de segurança padronizado e gerenciado centralmente, com
  visibilidade via FortiAnalyzer
