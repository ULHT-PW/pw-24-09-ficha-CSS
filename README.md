Universidade Lusófona
**Programação Web**

# Ficha 9: Estilização das aplicações com CSS, seus seletores e propriedades 

### Objetivo:
* Familiarizar-se com os selectores CSS 
* familiarizar-se com algumas propriedades CSS
* Irá usar a aplicação Bandas para experimentar todos os seletores e propriedades que falámos. Poderá ficar extra-colorida-folcórica, mas o intuito é experimentar! Noutra ficha terá oportunidade de estilizar a app do curso de forma mais coerente e sóbria. 

### Recomendações:
* consultar os slides da aula, lendo os restantes slides sobre propriedades CSS (slide 18 até ao fim).

# Estilização da aplicação Bandas 🎸
* crie na pasta da aplicação `bandas` a pasta `static/bandas`, onde guarde o ficheiro estilos.css.
* integre um link no layout.html base da aplicação.
* insira no layout.html, no elemento `<style>`, um bloco {% block style %} que permita integrar regras CSS específicas para algumas páginas da sua aplicação.
 
## Seletores CSS
* Para cada um dos selectores class, id, atributo, pseudo-classe e pseudo-elemento, deverá ter pelo menos 3 regras de cada (3 classes, 3 ids, etc) que apliquem estilos em sítios diferentes. 
* Utilize pelo menos três combinadores de selectores (descendentes, filhos `>`, adjacentes `~`, imediatamente adjacentes `+`, agrupados `,`). 
* De seguida dão-se algumas sugestões de elementos a estilizar.
 
## Estilização de elementos

#### Fonte
Escolha uma [fonte Google](https://fonts.google.com/) a seu gosto para as páginas da sua aplicação:
* no site, escolha uma fonte que goste
* clique em *add font*
* selecione *get embeded code*
* copie o código da página (três elementos link, como apresentados em baixo para a fonte Montserrat) e insira-os no elemento `<head>` do seu layout.html.
```css
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap" rel="stylesheet">
```
* insira no seu ficheiro css, uma regra com um selector universal e a declaração `font-family: "Montserrat", sans-serif;` de modo a que a fonte seja usada em todo o lado* Configure a cor de background do seu website, assim como de alguns elementos HTML5 usando seletores adequados. 

#### Menu
* Para o texto do menu, utilize os selectores de pseudo-classe `link`, `visited`, `hover`, `active` para configurar os links utilizando apenas as cores da palete, assim como os selectores `before` e `after` no menu quando passar com o rato por cima.
* Inclua, antes de cada palavra do menu, um icon adequado, usando ícones de Font Awesome. Para tal:
   * visite o [link](https://fontawesome.com/start)
   * registe-se para obter uma chave (por exemplo, `5d1319edfb`), 
   * no elemento head do layout.html, insira um elemento script   
`    <script src="https://kit.fontawesome.com/5d1319edfb.js" crossorigin="anonymous"></script>`
   * utilize [icons](https://fontawesome.com/search?q=music&o=r) a seu gosto. Para um icon à sua escolha (que não seja Pro, exclusivos para subscrições pagas) use no seu HTML o elemento que o identifica, por exemplo<br>`<i class="fa-solid fa-music"></i>`

#### Letras
* adicione, à classe Musica, o campo letra, um TextField. Não se esqueça de especificar os atributos default, null e blank:<br> `letra = models.TextField(default='', null=True, blank=True)`
* garanta que no formulário para inserir uma música aparece o campo letra.
* Insira a letra de pelo menos uma música por disco.
* evidencie, na lista de músicas de um disco, a música que tem letra, usando por exemplo um icon de Font Awesome.
* Na página da música, se existir, insira a letra.

#### Biografia
* adicione, à classe Musica, o campo biografia, um TextField.
* garanta que no formulário para inserir uma música aparece o campo biografia.
* Insira para cada banda uma biografia, peça ao chatGPT uma curta de 4-5 linhas.
* Na página da banda, insira a biografia.
* use selectores pseudo-elementos de first-letter e first-line para estilizar o texto da biografia.
11. nos seus formulários, remova o uso de quebras de linha `br` para colocar inputs em linhas diferentes. Em vez disso, transforme os elementos `input` em blocos através da propriedade `display`. 

### Fotografia da banda
* estilize as molduras (border) das imagens usando seletores, sem recorrer a classes.
* utilize mais do que uma cor para cada lado, ou só uma borda de cor de um dos lados.

### Formulários
* no forms.py, defina `help_texts` para todos os campos do formulário de nova banda, textos explicativos adicionais para os campos dos seus modelos.
* Exemplo: 
        help_texts = {
            'biografia': 'Insira uma breve biografia de 4-5 linhas.'
        }
* este texto é exibido junto ao campo biografia, no formulário, dentro de um elemento com o atributo `class="helptext"`.
* estilize-os usando CSS (por exemplo, use letras mais pequenas com a propriedade `font-size` e numa cor mais clara).


# Página HTML5 & CSS

* Crie uma nova página HTML `html5-css.html`.
* Insira um elemento `h3` com o título "Seletores CSS" onde deverá incluir:
    1. uma frase introdutória sobre CSS 
    2. uma tabela onde tem, na primeira coluna, todos os tipos de seletores CSS, um por linha. Na segunda coluna deverá indicar se o usou ou não nalguma página, recorrendo a um icon adequado (use os icones Google), e na terceira coluna deverá incluir um breve comentário a explicar como este funciona e onde o utilizou, colocando um link. 
* Insira um elemento `h3` com o título "Combinadores de seletores" onde deverá incluir:
    * uma tabela com todos os combinadores de seletores apresentados na aula, um por linha.
    * Na segunda coluna deverá indicar se o usou ou não nalguma página, recorrendo a um icon adequado (use os icones Google)
    * na terceira coluna deverá incluir um breve comentário a explicar como este funciona e onde o utilizou.


# Submissão
* submeta o link para a sua aplicação
