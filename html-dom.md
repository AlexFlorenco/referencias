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

    - ### Pelo seletor CSS
    ```
    document.querySelectorAll("SELETOR");
    ```
    > Deve-se passar o seletor no parâmetro (".classe", "#id", "tag").<br>
    > Retorna um vetor de objetos com todos os elementos encontrados.

    - ### Encontrando coleções de objetos
    ```
    document.OBJETO;
    ```
    > Retorna um vetor de objetos com todos os elementos encontrados. <br>
    > [Objetos HTML que são acessíveis](https://www.w3schools.com/js/js_htmldom_elements.asp#:~:text=The%20following%20HTML%20objects%20(and%20object%20collections)%20are%20also%20accessible%3A)

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

    - ### Adicionar um elemento HTML 
    ```
    ELEMENTO_PAI.appendChild(ELEMENTO_NOVO);
    ```
    > ### Por que é necessário aspas no parâmetro createElement() e no appendChild() não?
    > O parâmetro de entrada deve ser um objeto já existente, portanto se trata de uma referenciação, e não uma declaração.

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
    - ### Adicionando manipuladores
    ```
    document.getElementById("ID").EVENTO = FUNÇÃO;	
    ```
    ```
    ELEMENTO.addEventListener("EVENTO", FUNÇÃO);
    ```
    > [Todos os eventos do HTML DOM](https://www.w3schools.com/jsref/dom_obj_event.asp)<br>
    > Se necessário passar parâmetros, use uma função anônima para chamar sua função com parâmetros.
    >> ```ELEMENTO.addEventListener("EVENTO", function() { FUNÇÃO(PARÂMETROS) });```

    - ### Removendo manipuladores
    ```
    ELEMENTO.removeEventListener("EVENTO", FUNÇÃO);
    ```

    <br>

- ## Objeto document DOM
    ```
    let url = document.OBJETO;
    ```
    > [Todas as propriedades e métodos do objeto documento](https://www.w3schools.com/jsref/dom_obj_document.asp)

    <br>

- ## Nós
    - ### Propriedades de nós
        - NÓ.nodeName: Nome do nó;<br><br>
        - NÓ.nodeValue: Valor nó;<br><br>
        - ELEMENTO.nodeType: Tipo do nó.
            > 1 = Nó de elemento<br>
            2 = Nó de atributo (Descontinuado)<br>
            3 = Nó de texto<br>
            8 = Nó de comentário

    <br>

    - ### Navegação entre nós
        - ELEMENTO.parentNode: Retorna o nó pai;<br><br>
        - ELEMENTO.childNodes: Todos os nós filhos;
            > Retorna espaços em branco e comentários.<br> Solução: *children*
        - ELEMENTO.firstChild: Primeiro nó filho;
            > Retorna espaços em branco e comentários.<br> Solução: *firstElementChild*
        - ELEMENTO.lastChild: Último nó filho;
            > Retorna espaços em branco e comentários.<br> Solução: *lastElementChild*
        - ELEMENTO.nextSibling: Próximo nó irmão;
            > Retorna espaços em branco e comentários.<br> Solução: *nextElementSibling*
        - ELEMENTO.previousSibling: Nó irmão anterior.
            > Retorna espaços em branco e comentários.<br> Solução: *previousElementSibling*