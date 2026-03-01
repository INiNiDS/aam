---
sidebar_position: 1
title: "Introdução"
---

# AAM (Abstract Alias Mapping)
## Apresentando o AAM
Os ficheiros de configuração têm tendência para crescer de forma descontrolada. Tornam-se volumosos, difíceis de ler, e ainda mais difíceis de manter. Dividi-los em múltiplos ficheiros ajuda, mas não resolve a complexidade subjacente de gerir relações de dados. Precisávamos de uma forma mais intuitiva de gerir mapeamentos — precisávamos do AAM.
### O problema - Mapeamento Verboso
Imagine que precisa de gerir um grande conjunto de aliases bidirecionais (onde pode procurar uma chave pelo valor e vice-versa). Em formatos como TOML, é forçado a usar muito código boilerplate:
```toml
[alias]
a = "b"
b = "a"
```
São três linhas para um único mapeamento. Multiplique isso por cem, e a sua configuração torna-se um pesadelo.
### A solução - AAM
O AAM é uma sintaxe simples e elegante que permite definir mapeamentos bidirecionais numa única linha. Com AAM, pode escrever:
```aam
a = b
```
Esta única linha cria um mapeamento bidirecional entre `a` e `b`. Pode procurar `a` para obter `b`, e procurar `b` para obter `a`. É conciso, claro, e elimina o boilerplate.
O AAM foi concebido para ser conciso, legível e fácil de usar, eliminando o boilerplate para que se possa concentrar na lógica da sua configuração.
## Como surgiu a ideia
Estava a trabalhar num projeto que me exigia gerir um grande número de aliases. Estava a usar TOML para os meus ficheiros de configuração, e apercebi-me de que era muito difícil gerir os meus aliases. Tinha de escrever muito código boilerplate para gerir os meus aliases, e era muito fácil cometer erros. Queria uma forma melhor de gerir os meus aliases, e foi assim que surgiu a ideia do AAM.
## Começar
Pronto para simplificar as suas configurações? Consulte o [Guia de Início Rápido](using/getting-started) para aprender a usar o AAM nos seus projetos.
