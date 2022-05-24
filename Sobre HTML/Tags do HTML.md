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