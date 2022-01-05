---
title: Admonition
publish: true
notetype: feed
cssclass: admonitions
date: 05-01-2022
tags: plugin
---

> Adiciona um bloco personalizado de conteúdo estilizado ao estilo [Material for MKDOCS](https://cutt.ly/aUXAzRZ)

- [b] [Github](https://github.com/valentine195/obsidian-admonition) 

# Sintaxe
Adicione um bloco de código com o tipo `ad-TIPO_DESEJADO` após isso alguns parâmetros podem ser determinados:

| Parâmetro       | Opções                                                  | OBS                                                     |
| --------------- | ------------------------------------------------------- | ------------------------------------------------------- |
| icon            | Nome do Ícone dos tema **FontAwesome** e **RPGAwesome** | Altera o ícone                                          |
| color           | Tríade RGB. Ex.: 200, 200, 200                          | Altera a cor                                            |
| NENHUM CONTEÚDO |                                                         | Se ficar em branco ele irá renderizar somente um titulo |
| title           | Texto                                                   | Titulo                                                        |

## Tipos
Os seguintes tipos são suportados como padrão:

| Tipo     | Alias                       |
| -------- | --------------------------- |
| note     | note, seealso               |
| abstract | abstract, summary, tldr     |
| info     | info, todo                  |
| tip      | tip, hint, important        |
| success  | success, check, done        |
| question | question, help, faq         |
| warning  | warning, caution, attention |
| failure  | failure, fail, missing      |
| danger   | danger, error               |
| bug      | bug                         |
| example  | example                     |
| quote    | quote, cite                 | 


# Bloco de Códigos
Blocos de códigos podem ser renderizados dentro do admonition de duas formas. Adicionando ele dentro do bloco Admonition como se fosse um simples bloco na modalidade Agrupamentos/Aninhado/Nested, ou para uma linha simples desde que adicione-se um parâmetro `~~~LINGUAGEM_QUE_O_CODIGO_FOI_ESCRITO` antes do código e após `~~~`. Ex.:

````ad-info

```ad-bug
title: Código em Linha Simples
~~~javascript
throw new Error("Oops, I'm a bug.");
~~~
```

Código em forma de bloco
```javascript
console.log("Hello!");
```

````

# Agrupamentos
Blocos podem ser aninhados/agrupados um dentro do outro como o exemplo abaixo

`````ad-note
title: Nested Admonitions
collapse: open

Hello!

````ad-note
title: This admonition is nested.
This is a nested admonition!

```ad-warning
title: This admonition is closed.
collapse: close
```

````

This is in the original admonition.
`````



# Referências
- Web
	- [Font Awesome](https://fontawesome.com/)
	- [RPG-Awesome | A fantasy themed font and CSS toolkit](https://nagoshiashumari.github.io/Rpg-Awesome/)
	- [Admonitions - Material for MkDocs](https://squidfunk.github.io/mkdocs-material/reference/admonitions/)

	