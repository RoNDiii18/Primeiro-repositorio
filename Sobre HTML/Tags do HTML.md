Parágrafos

**Como criar parágrafos?**

Para se declarar parágrafos em páginas pode-se utilizar a tag <p>. Entretanto, é possível aplicar diversos tipos de formatações a parágrafos. Veja o exemplo a seguir:

```
<p>    
    <b>Texto em negrito</b><br>
    <i>Texto em itálico</i><br>
    <u>Texto sublinhado</u><br>
    <sub>Texto subscrito</sub><br>
    <sup>Texto sobrescrito</sup><br>
    <big>Texto com fonte maior do que o padrão</big><br>
    <small>Texto com fonte menor do que o padrão</small><br>
    <em>Texto em itálico</em><br>
    <strong>Texto em negrito</strong>
</p>
```

Ao exibir nosso código em um navegador veremos o seguinte resultado:

![img](https://img-c.udemycdn.com/redactor/raw/2018-04-03_13-24-49-baa1faa6ff4ed0b49d1e52f9d71153e7.jpg)



Podemos ainda alterar a fonte usando o atributo style e a propriedade font-family:

```
<!-- Declarando uma única fonte -->
<p style="font-family: 'Times New Roman'">Olá, mundo!</p>

<!-- Declarando duas possíveis fontes -->
<p style="font-family: 'Helvetica, Arial'">Olá, mundo novamente!</p>
```



Observe que o trecho...

```
<!-- Declarando uma única fonte -->
```

... não é mostrado na tela do navegador. Use os símbolos de <!-- e --> para inserir comentários. Comentários permitem a organização do código.



**Quebras de linha**

Podemos usar a tag <br> para inserir quebras de linha em nossa página.



**Tags de títulos**

São 6 ao todo:

```
<h1>Título 1</h1>

<h2>Título 2</h2>

<h3>Título 3</h3>

<h4>Título 4</h4>

<h5>Título 5</h5>

<h6>Título 6</h6>
```

# Estilos

Estilos permitem que sua página tenha diversos tipos de formatações. Eles podem ser declarados com o atributo style (como mostrado anteriormente) ou com a tag <style>.

No exemplo a seguir vamos demonstrar como alterar a cor de um texto:

```
<style>
p { color: red; }
</style>
```

Esse exemplo aplica a cor vermelha a todos os elementos do tipo parágrafo.

Podemos ainda aplicar cores ao fundo. Observe o exemplo a seguir:

```
<style>
body { background-color: red; }
</style>
```

Nesse exemplo, o plano de fundo da página foi alterado para a cor vermelha.

Agora vamos construir uma página completa aplicando estilos:

```
<!DOCTYPE html>
<html>
<head>
    <title>Meus estilos</title>
    <style>
        body {             
        background-color: red;
        color:green;
      
        }
    </style>
    </head>
    
    <body>
    
        <p>Olá mundo</p>
    
    </body> </html>
```



Veja que a tag <style> deve ser declarada dentro da tag <head>. 



a tag "width" altera o comprimento da imagem

a tag "height" altera a altura da imagem



Linhas horizontais e listas

Podemos adicionar linhas horizontais usando a tag <hr>.

```
<hr>
```

Listas podem ser criadas usando a tag <ul> (listas não ordenadas) ou <ol> (listas ordenadas) e cada elemento pode ser inserido com a tag <li>.

```
<!-- Lista ordenada -->
<ol>
<li>Primeiro elemento</li>
<li>Segundo elemento</li>
<li>Terceiro elemento</li>
</ol>
<!-- Lista não ordenada --><ul>
<li>Primeiro elemento</li>
<li>Segundo elemento</li>
<li>Terceiro elemento</li>
</ul>
```

![img](https://img-c.udemycdn.com/redactor/raw/2018-04-03_13-27-35-d27f66b1c05eb8f2c4b2aa2e2ab15e6a.jpg)



Tabelas

Podemos criar tabelas usando a tag <table>. 

Cada linha deve ser declarada com a tag <tr> e cada célula com a tag <td>. 

Opcionalmente podemos usar a tag <th> para declarar células que representem a linha de cabeçalho.

![img](https://img-c.udemycdn.com/redactor/raw/2018-04-03_13-32-10-36b8389078e5ece1ff797ca7e15d38d1.jpg)



Estruturas de um website

Para que websites sejam bem desenvolvidos, existe um conjunto de tags que indicam onde cada conteúdo deve ser inserido. Em geral, essas tags são apenas estruturais, ou seja, ao serem inseridas, não trazem modificações a estrutura da página. 

Observe a seguir algumas tags estruturais:

![img](https://img-c.udemycdn.com/redactor/raw/2018-03-17_14-04-44-4622827886bf69cce0fd0ca735eb1c5c.png)

 Destaco a tag <div>. Essa tag permite a inserção de divisórias nas páginas, ou seja, são tags estruturais que permitirão que você organize seu código.

```
<div> 
    <p>Conteúdo de uma div</p>
</div>
```

Construindo uma página completa

**Construindo uma página completa**

Nesta aula vamos aprender a construir uma página completa. Vamos usar como exemplo a página demonstrada na aula "Estruturas de um Website".

![img](https://img-c.udemycdn.com/redactor/raw/2018-03-17_14-04-44-4622827886bf69cce0fd0ca735eb1c5c.png)

Agora, vamos criar a estrutura desta página usando HTML: 

```
<!DOCTYPE html>
<html>
<head>

    <title>Página completa</title>
    <meta charset="UTF-8">
    
</head>

<body>

    <!-- Cabeçalho -->
    <header>
       
        <nav></nav>
    </header>
    
    <!-- Conteúdo -->
    <div>
    
        <article>
            <section></section>
        </article>
        
        <aside></aside>
        
     </div>
     
     <!-- Rodapé -->
     <footer></footer>
     </body>
     
     </html>
```

Ao implementar isso, você não verá modificação alguma.

Alterando as cores

> #### <style> cores </style>

Você pode alterar as cores de seu texto e de sua página com a tag <style>.

Para isso devemos aplicar as chamadas propriedades:

> **color**: altera a cor do texto
>
> **background-color**: altera a cor de fundo



Para isso, você deve adicionar o nome da cor em inglês ou o código RGB. Por exemplo:

```
<html>
<head>
<style>
    body{
        color: red;
        background-color:#FFFFFF;
    }
</style>
</head>
<body>
Olá mundo!
</body>
</html>
```



> Vamos tentar entender o código:

A tag style aplica um determinado estilo à página. No caso, você aplicou um estilo a tudo que estiver no body. A cor aplicada ao texto é vermelha (red) e ao fundo é branco (#FFFFFF).

**Resumo**

**O que é HTML?**

> **HTML** (*Hypertext Markup Language* ou na tradução para o português Linguagem de Marcação de Hipertexto) é uma linguagem utilizada para construção de páginas de Internet. HTML define um conjunto de regras que permite a formatação de páginas. Um documento HTML consiste em um arquivo de texto que será lido e interpretado como uma página por browsers (navegadores), como por exemplo, Chrome, Firefox, Opera, Edge ou Safari.

Páginas HTML possuem elementos de marcação, chamados de tags, que indicam como a página deverá ser formatada. Tags são indicadas entre os símbolos de <>.

Abaixo temos o exemplo do código de uma simples página HTML:

```
<!DOCTYPE html>
<html>
    <head>
        <title>Hello</title>
    </head>
    
    <body>
    <p>Olá, mundo!</p>
    </body>
</html>
```



**Como declarar imagens?**

Você pode declarar imagens usando a tag <img>. O endereço de uma imagem, isto é, a localização da imagem deverá ser indicada pelo atributo src.

<img src="foto.jpg"> 

**Como declarar links?**

Links permitem que o usuário navegue de uma página a outra. Devem ser declarados com a tag <a>.

<a href="pagina_2.html">Link para a página 2</a> 

**Como declarar formulários?**

Formulários permitem que o usuário envie dados para um sistema web. Devem ser declarados com a tag <form>. O atributo action indica a página que será carregada. O método de envio pode ser "post" (mais recomendado) ou "get" (envio pela url).

```
<form action="recebe.php" method="post" name="form"></form>
```

> Tipos entradas <input> para formulários:

- **text**: texto
  - <input type="text>
- **password**: senhas
  - <input type="password>
- **hidden**: campo oculto
  - <input type="hidden>
- **checkbox**: caixa de marcação
  - <input type="checkbox>