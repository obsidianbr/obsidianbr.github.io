---
title: Dataview
publish: true
notetype: feed
date: 12-12-2021
tags: plugin
---

Dataview é um dos mais úteis e populares plugins do Obsidian, ele é capaz de transformar a base de notas criadas pelo usuário em um verdadeiro banco de dados. Possui uma 2 formas básicas de trabalho, sendo uma primeira mais simples baseado em consultas SQL comuns e uma segunda forma através de uma robusta API Javascript.

# Links Úteis

- [Github Oficial (em Inglês)](https://github.com/blacksmithgu/obsidian-dataview)
- [Documentação oficial (em Inglês)](https://blacksmithgu.github.io/obsidian-dataview/)
- [Forum oficial do Obsidian com exemplos de uso do Dataview (em Inglês)](https://forum.obsidian.md/t/dataview-plugin-snippet-showcase/)
- [Forum oficial do Obsidian com exemplos de uso do DataviewJS  (em Inglês)](https://forum.obsidian.md/t/dataviewjs-snippet-showcase)


# Dataview
Para o uso do dataview dentro de uma nota no Obsidian, deve-se obedecer a seguinte sintaxe:

```
dataview
TABLE|LIST|TASK <field> [AS "Column Name"], <field>, ..., <field> FROM <source> (like #tag or "folder")
WHERE <expression> (like 'field = value')
SORT <expression> [ASC/DESC] (like 'field ASC')
... other data commands
```

Importante que o código da pesquisa desejada esteja dentro de um cloco de códigos e na primeira linha contenha a palavra dataview

## Exemplos

Lista todas as notas que contenham as **tags** games/mobas ou games/crpg:

```
dataview
LIST FROM #games/mobas OR #games/crpg
```

