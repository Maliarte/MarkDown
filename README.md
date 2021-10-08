#### Tradução realizada por MEID para Estudo de Markdown.

Markdown é uma linguagem simples de marcação originalmente criada por John Gruber e Aaron Swartz. Markdown converte seu texto em HTML válido. 
Markdown é frequentemente usado para formatar arquivos README, para escrever mensagens em fóruns de discussão online e para criar rich text 
usando um editor de texto simples.

:smiling_face_with_three_hearts: repositório origem: [Markdown CheatSheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)


### Pretende ser uma referência rápida e uma demonstração. Para obter informações mais completas, consulte as especificações originais de John Gruber e a página de informações do Markdown com sabor do Github.


Sumário

* Cabeçalhos
* Ênfase
* Listas
* Links
* Imagens
* Destaque de código e sintaxe
* Mesas
* Citações em bloco
* HTML embutido
* Regra Horizontal
* Quebras de linha
* Vídeos do YouTube

####  Cabeçalhos

`# H1 `
`## H2 `
`### H3`
`#### H4`
`##### H5`
`###### H6 `

* # H1 
* ## H2 
* ### H3
* #### H4
* ##### H5
* ###### H6 


#### Ênfase | Emphasis

## Ênfase, também conhecido como itálico, com asteriscos ou sublinhados.

Emphasis, aka italics, with *asterisks* or _underscores_.

## Ênfase forte, também conhecida como negrito, com asteriscos ou sublinhados.
Strong emphasis, aka bold, with **asterisks** or __underscores__.

## Ênfase combinada com asteriscos e sublinhados.
Combined emphasis with **asterisks and _underscores_**.

## O tachado usa dois til. 
Strikethrough uses two tildes. ~~Scratch this.~~


## Listas | Lists

(Neste exemplo, os espaços à esquerda e à direita são mostrados com pontos: ⋅)

1. Primeiro item da lista pedido
2. Outro item
⋅⋅* Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number Os números reais não importam, apenas que é um número
⋅⋅1. Ordered sub-list
4. And another item. E outro item


### Você pode ter parágrafos recuados corretamente nos itens da lista. Observe a linha em branco acima e os espaços iniciais (pelo menos um, mas usaremos três aqui para também alinhar o Markdown bruto).

⋅⋅⋅You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).


### ⋅⋅⋅Para ter uma quebra de linha sem parágrafo, você precisará usar dois espaços finais.⋅⋅ ⋅⋅⋅Note que esta linha é separada, mas dentro do mesmo parágrafo.⋅⋅ ⋅⋅⋅ (Isso é contrário ao comportamento típico de quebra de linha GFM, em que espaços à direita não são necessários.)

⋅⋅⋅To have a line break without a paragraph, you will need to use two trailing spaces.⋅⋅
⋅⋅⋅Note that this line is separate, but within the same paragraph.⋅⋅
⋅⋅⋅(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

`* Unordered list can use asterisks`\
`- Or minuses `\
`+ Or pluses`



####  Links

Existem dois jeitos de criar links

[Sou um link de estilo embutido](https://www.google.com)

[Sou um link de estilo embutido com título](https://www.google.com "Google's Homepage")

[Eu sou um link de estilo de referência][Arbitrary case-insensitive reference text]

[Sou uma referência relativa a um arquivo de repositório(../blob/master/LICENSE)

[Você pode usar números para definições de link de estilo de referência][1]

Ou deixe-o vazio e use o [link text itself].

URLs and URLs in angle brackets will automatically get turned into links. 
http://www.example.com or <http://www.example.com> and sometimes 
example.com (but not on Github, for example).

Some text to show that the reference links can follow later.

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com

Here's our logo (hover to see the title text):

Inline-style: 
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

Reference-style: 
![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"


Destaque de código e sintaxe

Os blocos de código são parte da especificação do Markdown, mas o destaque de sintaxe não. No entanto, muitos renderizadores - como Github's e Markdown Here - suportam realce de sintaxe. Quais idiomas são suportados e como esses nomes de idioma devem ser escritos variam de renderizador para renderizador. Markdown Here suporta realce para dezenas de idiomas (e não-realmente-idiomas, como diffs e cabeçalhos HTTP); para ver a lista completa e como escrever os nomes dos idiomas, consulte a página de demonstração highlight.js.

Aplicação:
Inline `code` has `back-ticks around` it.

//codigo embutido tem "`" 

Os blocos de código são delimitados por linhas com três back-ticks `` `, ou são indentados com quatro espaços. Eu recomendo usar apenas os blocos de código protegidos - eles são mais fáceis e apenas suportam o realce de sintaxe.


```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
 
```python
s = "Python syntax highlighting"
print s
```
 
```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```


####  Tabelas

As tabelas não fazem parte das especificações básicas do Markdown, mas fazem parte do GFM e o Markdown Aqui as suporta. Eles são uma maneira fácil de adicionar tabelas ao seu e-mail - uma tarefa que, de outra forma, exigiria copiar e colar de outro aplicativo.

    Colons can be used to align columns. Os dois pontos podem ser usados ​​para alinhar colunas.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the 
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less      | Pretty
     --- | ---       | ---
*Still*  | `renders` | **nicely**
1        | 2         | 3


Blockquotes | Citações em bloco
> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote. 

####  Inline HTML

Você também pode usar HTML bruto em seu Markdown e, na maioria das vezes, funcionará muito bem.
<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>

Regra Horizontal | Horizontal Rule

Three or more...

---

Hyphens

***

Asterisks

___

 Underscores 


### Quebras de linha | Line Breaks

Minha recomendação básica para aprender como as quebras de linha funcionam é experimentar e descobrir - pressione <Enter> uma vez (ou seja, insira uma nova linha), depois pressione duas vezes (ou seja, insira duas novas linhas), para ver o que acontece. Em breve, você aprenderá a conseguir o que deseja. "Markdown Toggle" é seu amigo.

Aqui estão algumas coisas para experimentar:

Aqui está uma linha para começarmos.

Esta linha é separada da anterior por duas novas linhas, portanto, será um * parágrafo separado *.

Esta linha também é um parágrafo separado, mas ...
Esta linha é separada apenas por uma única nova linha, portanto, é uma linha separada no * mesmo parágrafo *.

####  YouTube Videos  

Eles não podem ser adicionados diretamente, mas você pode adicionar uma imagem com um link para o vídeo como este:

<a href="http://www.youtube.com/watch?feature=player_embedded&v=YOUTUBE_VIDEO_ID_HERE
" target="_blank"><img src="http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

Ou, em puro Markdown, mas perdendo o tamanho e a borda da imagem:

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](http://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID_HERE)\
  
  :blue_heart:
