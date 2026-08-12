---
title: Planejamento e criação de novo Datacenter — Grupo Belarmino (2019)
tipo: projeto
area: redes
status: concluido
publish: true
tags: [redes, infraestrutura, datacenter, virtualizacao, storage, alta-disponibilidade]
data: 2019
empresa: Grupo Belarmino
stack: [VMware vSphere, HP Storage, Fiber Channel, Sonicwall]
---

# Planejamento e criação de novo Datacenter — Grupo Belarmino (2019)

## Contexto
Planejamento, desenvolvimento e criação de um novo Datacenter central de
alta disponibilidade para o Grupo Belarmino, com acesso a mais de 90
localidades. Esse foi o Datacenter que, posteriormente, seria fisicamente
transferido para Campinas-SP (projeto de move de Datacenter, 2020).

## Meu papel
Planejei, desenvolvi e criei o Datacenter central descrito abaixo.

## Objetivo
Criar um Datacenter central de alta disponibilidade, capaz de atender com
acesso a mais de 90 localidades, com redundância em todas as camadas
críticas: virtualização, storage, links, firewall e energia.

## O que foi feito
- Planejamento, desenvolvimento e criação de Datacenter central com alta
  disponibilidade, com acesso para mais de 90 localidades
- Virtualização em **VMware vSphere**
- Storage **HP** em **Fiber Channel**
- Redundância de links de comunicação
- Firewall **Sonicwall** com HA (alta disponibilidade)
- Redundância física de energia, com no-breaks (UPS) redundantes e gerador
  de grande porte como backup

## Resultados
- Datacenter central de alta disponibilidade em operação, atendendo mais
  de 90 localidades
- Redundância completa em virtualização, storage, links, firewall e energia
- Base de infraestrutura que sustentou a operação até a posterior migração
  física do Datacenter, em 2020
