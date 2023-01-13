# Referência HTML DOM

- ## Encontrando elementos HTML
    - ### Pelo ID
    ```
    document.getElementById("ID");
    ```

    - ### Pela tag
    ```
    document.getElementsByTagName("TAG");
    ```
    > Retorna um vetor de objetos com todos os elementos encontrados.

    - ### Pela classe
    ```
    document.getElementsByClassName("CLASSE");
    ```
    > Retorna um vetor de objetos com todos os elementos encontrados.

<br>

- ## Alterando elementos HTML
    - ### Alterar o conteúdo
    ```
    ELEMENTO.innerHTML = "CONTEÚDO";
    ```

    - ### Alterar o estilo
    ```
    ELEMENTO.style.PROPRIEDADE = "VALOR";
    ```

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

- ## Adicionando ou deletando elementos
    - ###
    ```

    ```
    >