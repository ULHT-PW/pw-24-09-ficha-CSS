Universidade Lusófona
**Programação Web**

# Ficha 9: Estilização das aplicações com seletores e propriedades CSS 

### Objetivo:
* Familiarizar-se com os selectores CSS 
* familiarizar-se com algumas propriedades CSS

### Recomendações:
* consultar os slides da aula
* ver os restantes slides sobre propriedades CSS

# 3. Página HTML5 & CSS

1. Crie uma nova página HTML `html5-css.html` que tenha o mesmo cabeçalho das restantes.
2. Insira um elemento `h3` com o título HTML5 e CSS. Esta página terá 3 secções, estruturadas com elementos `section`, onde cada uma terá um breve texto e uma tabela. 
3. Crie uma secção com o elemento intitulada HTML 5 onde deverá incluir:
    1. uma frase introdutória sobre o HTML5
    2. um tabela com :
       * na primeira coluna todos os elementos HTML5 apresentados na aula, um por linha. 
       * na segunda coluna, para cada elemento HTML5 deverá indicar se o usou ou não nalguma página, recorrendo a um icon adequado (use os icones Google)
       * na terceira coluna deverá incluir uma breve descrição a explicar onde utilizou. 
4. Crie uma subsecção intitulada CSS onde deverá incluir:
    1. uma frase introdutória sobre CSS 
    2. uma tabela com todos os tipos de seletores CSS, um por linha. Na segunda coluna deverá indicar se o usou ou não nalguma página, recorrendo a um icon adequado (use os icones Google), e na terceira coluna deverá incluir um breve comentário a explicar como este funciona e onde o utilizou. 
    3. uma tabela com todos os combinadores de seletores apresentados na aula, um por linha. Na segunda coluna deverá indicar se o usou ou não nalguma página, recorrendo a um icon adequado (use os icones Google), e na terceira coluna deverá incluir um breve comentário a explicar como este funciona e onde o utilizou.

# 4. Estilização das aplicações com CSS

Para a definição dos estilos será usado um único ficheiro estilos.css, que guardará todos os estilos usados nas páginas. Em cada ficheiro HTML deverá existir um link para este ficheiro, de modo a permitir usar os estilos.

1. crie o ficheiro estilos.css 
2. deverá utilizar todos os tipos seletores apresentados na aula em pelo menos 3 sitios diferentes. 
3. Deverá utilizar pelo menos três composições de selectores (descendentes, filhos `>`, adjacentes `~`, imediatamente adjacentes `+`, agrupados `,`). 
4. Para o texto do menu, deverá utilizar os selectores de pseudo-classe `link`, `visited`, `hover`, `active` para configurar os links utilizando apenas as cores da palete, assim como os selectores `before` e `after` no menu quando passar com o rato por cima. Inclua, antes de cada palavra do menu, um icon adequado, usando ícones Google, Awesome Font ou Bootstrap. 

6. Configure a cor de background do seu website, assim como de alguns elementos HTML5 usando seletores adequados. 
7. Em particular nas tabelas e no poema os selectores de pseudo-classe assim como os pseudo-elementos, explorando cores de fonte e fundos diferentes. Por exemplo, introduza variedades de cor nas linhas pares e impares das tabelas.
9. Deverá recorrer aos 6 seletores de atributo `=`, `~=`, `|=`, `^=`, `$=` e `*=` para configurar as cores e larguras das molduras em redor das imagens da página interesses.
10. No texto descritivo, use os pseudo-elementos first-letter, first-line para estilizá-lo.
11. nos seus formulários, remova o uso de quebras de linha `br` para colocar inputs em linhas diferentes. Em vez disso, transforme os elementos `input` em blocos através da propriedade `display`. 
12. No formulário de comentário, atualize a informação relativa ao elemento escondido, que deverá indicar que o comentário é referente ao lab 4.
13. estilize as molduras (border) das imagens e iframes usando seletores, sem recorrer a classes.


# A. aplicação web bandas 🎸
* crie na pasta da aplicação `bandas` a pasta `static/bandas`, onde guarde o ficheiro estilos.css.
* integre um link no layout.html base da aplicação.
* insira no layout.html, no elemento `<style>`, um bloco {% block style %} que permita integrar regras CSS específicas para algumas páginas da sua aplicação.
* Escolha uma [Google Font](https://fonts.google.com/) a seu gosto para a sua aplicação, criando uma regra com um seletor universal de modo a que seja usada em todo o lado:
   * no site escolha uma fonte que goste
   * clicke em add font
   * selecione "get embeded code"
   * copie o código da página (três elementos link, como apresentados em baixo) e insira-os no elemento `<head>` do seu layout.html.

```css
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap" rel="stylesheet">
```
   * insira no ficheiro css `font-family: "Montserrat", sans-serif;`
 
* Para cada um dos selectores class, id, atributo, pseudo-classe e pseudo-elemento, deverá ter pelo menos 3 regras de cada (3 classes, 3 ids, etc) que apliquem estilos em sítios diferentes. 
* Utilize pelo menos três combinadores de selectores (descendentes, filhos `>`, adjacentes `~`, imediatamente adjacentes `+`, agrupados `,`). 
* Para o texto do menu, utilize os selectores de pseudo-classe `link`, `visited`, `hover`, `active` para configurar os links utilizando apenas as cores da palete, assim como os selectores `before` e `after` no menu quando passar com o rato por cima.
* Inclua, antes de cada palavra do menu, um icon adequado, usando ícones de Font Awesome. Para tal:
   * visite o [link](https://fontawesome.com/start)
   * registe-se para obter uma chave (por exemplo, `1234abcd`), 
   * use a chave, inserindo no elemento head um script 
`<script src="https://kit.fontawesome.com/1234abcd.js" crossorigin="anonymous"></script>`
   * utilize [icons](https://fontawesome.com/search?q=music&o=r) a seu gosto, usando o elemento que o identifica, por exemplo `<i class="fa-solid fa-music"></i>`

 

# B. aplicação artigos 📚
* Se o utilizador estiver autenticado e fizer parte do grupo, torne editáveis todos os dados (criar, alterar e remover elementos).

# C. aplicação curso 🎓
* Se o utilizador estiver autenticado e fizer parte do grupo, torne editáveis todos os dados (criar, alterar e remover elementos).



