# Referência HTML DOM

## Encontrando elementos HTML
- ### Pelo ID
```
document.getElementById("ID");
```

<br> 

- ### Pela tag
```
document.getElementsByTagName("TAG");
```
> Retorna um vetor de objetos com todos os elementos encontrados.

<br>

- ### Pela classe
```
document.getElementsByClassName("CLASSE");
```
> Retorna um vetor de objetos com todos os elementos encontrados.

<br>
<br>

## Alterando elementos HTML
- ### Alterar o conteúdo
```
ELEMENTO.innerHTML = "CONTEÚDO";
```

<br>

- ### Alterar o estilo
```
ELEMENTO.style.PROPRIEDADE = "VALOR";
```

<br>

- ### Alterar o atributo
```
ELEMENTO.ATRIBUTO = "VALOR";
> Propriedade 
```

```
ELEMENTO.setAttribute(ATRIBUTO, "VALOR");
> Método
```

> ### .attribute VS setAttribute()
> Os dois casos executam a mesma função, mas irão existir situações em que o atributo não faz parte do DOM, fazendo necessário o setAttribute().

<br>
<br>

## Adicionando ou deletando elementos
```

```
>