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

    <br>

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
    > [Todas as propriedades para objetos de estilo](https://www.w3schools.com/jsref/dom_obj_style.asp)

    <br>

    - ### Alterar o atributo
    ```
    ELEMENTO.ATRIBUTO = "VALOR";
    > Propriedade 
    ```
    ```
    ELEMENTO.setAttribute("ATRIBUTO", "VALOR");
    > Método
    ```
    > ### .attribute VS setAttribute()
    > Os dois casos executam a mesma função, mas irão existir situações em que o atributo não faz parte do DOM, fazendo necessário o setAttribute().

<br>

- ## Adicionando ou deletando elementos
    - ### Criar um elemento HTML
    ```
    document.createElement("ELEMENTO");
    ```
    > Cria um nó de elemento. Necessário adicionar conteúdo (inner) e setar o destino (append).

    <br>

    - ### Adicionar um elemento HTML 
    ```
    ELEMENTO_PAI.appendChild(ELEMENTO_NOVO);
    ```
    > ### Por que é necessário aspas no parâmetro createElement() e no appendChild() não?
    > O parâmetro de entrada deve ser um objeto já existente, portanto se trata de uma referenciação, e não uma declaração.

    <br>

    - ### Remover um elemento HTML
    ```
    ELEMENTO_PAI.removeChild(ELEMENTO_FILHO);	
    ```

    - ### Substituir um elemento HTML
    ```
    ELEMENTO_PAI.replaceChild(ELEMENTO_NOVO, ELEMENTO_FILHO);
    ```

    - ### Escrever no output HTML
    ```
    document.write("TEXTO");
    ```
    > O uso deste método é fortemente desencorajado.

    <br>

- ## Manipuladores de eventos
    ```
    document.getElementById("ID").EVENTO = function(){ }	
    ```
    > [Todos os eventos do HTML DOM](https://www.w3schools.com/jsref/dom_obj_event.asp)

    <br>

- ## Objetos do documento DOM
    ```
    let url = document.OBJETO;
    ```
    > [Todas as propriedades e métodos dos objetos de documento](https://www.w3schools.com/jsref/dom_obj_document.asp)

    <br>

- ##
    ```

    ```
    >