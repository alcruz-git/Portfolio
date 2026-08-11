---
title: Desenho e implementação de Active Directory único — Grupo Belarmino (2022)
tipo: projeto
area: redes
status: concluido
publish: true
tags: [redes, active-directory, iam, infraestrutura, microsoft]
data: 2022
empresa: Grupo Belarmino
stack: [Active Directory, Windows Server]
---

# Desenho e implementação de Active Directory único — Grupo Belarmino (2022)

## Contexto
O Grupo Belarmino é composto por várias empresas, cada uma originalmente com
sua própria estrutura de identidade e login. O projeto propôs unificar todas
elas em um único domínio Active Directory (GB), permitindo login único para
qualquer usuário em qualquer empresa do grupo.

## Meu papel
Realizei o desenho, a estruturação e a implementação completa do Active
Directory único do grupo.

## Objetivo
Unificar as identidades de todas as empresas do grupo em uma estrutura única
e de fácil utilização — inclusive para usuários que se deslocam entre
unidades — garantindo controle total de IAM a partir de uma única base de
identidades, também usada como base de IAM para os demais sistemas.

## O que foi feito
- Desenho, estruturação e implementação de um Active Directory único
  (domínio GB) para todo o Grupo Belarmino
- Unificação das múltiplas empresas do grupo em uma **floresta única**
- Estrutura de fácil uso para usuários que se deslocam entre unidades,
  com login único em qualquer empresa do grupo
- Base única de identidades, servindo também como base de IAM para os
  demais sistemas da organização
- Redundância por meio de um controlador de domínio por localidade
- Configuração de sites e site links por localidade, otimizando a
  velocidade de login local em cada unidade
- Implementação seguindo o framework e as melhores práticas da Microsoft,
  com administração centralizada

## Decisões técnicas e por quê
- Optar por uma floresta única, em vez de múltiplos domínios/florestas,
  simplificou a administração e garantiu controle de identidade
  centralizado em todo o grupo
- Um controlador de domínio por localidade, com sites e site links
  configurados, garantiu redundância e login local rápido mesmo mantendo
  a estrutura de domínio único

## Resultados
- Login único (SSO) disponível para usuários em qualquer empresa do grupo
- Base única de identidades, reaproveitada como IAM para outros sistemas
- Redundância local em cada unidade, via controlador de domínio próprio
- Velocidade de login otimizada por localidade
