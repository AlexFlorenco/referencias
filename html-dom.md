# Referência HTML DOM

### Encontrando elementos HTML
```
document.getElementById("ID");
```
> Retorna o elemento encontrado pelo id.

```
document.getElementsByTagName("TAG");
```
> Retorna um vetor de objetos com todos os elementos encontrado pela tag.

```
document.getElementsByClassName("CLASSE");
```
> Retorna um vetor de objetos com todos os elementos encontrado pela classe.


### Alterando elementos HTML
```
ELEMENTO.innerHTML = "CONTEÚDO";
```
> Altera o conteúdo do elemento.

```
ELEMENTO.style.PROPRIEDADE = "VALOR";
```
> Altera o estilo do elemento.

```
ELEMENTO.ATRIBUTO = "VALOR";
```
> Altera o atributo do elemento. (Propriedade)

```
ELEMENTO.setAttribute(ATRIBUTO, "VALOR");
```
> Altera o atributo do elemento. (Método)

>> ###.attribute VS setAttribute()
>>>Nos dois casos executam a mesma função, mas irão existir casos em que o atributo não faz parte do DOM.


### Adicionando ou deletando elementos
```

```
>