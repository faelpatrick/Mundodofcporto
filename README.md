# Atividade de Manipulação do DOM com JavaScript

## Objetivo
Realizar algumas tarefas para melhorar e corrigir o código HTML e JavaScript fornecido. 
Esta atividade ajudará a entender melhor integração de JavaScript com HTML.

## Instruções
Abra seu github, vá ate o ficheiro trofeus.html e aqui temos duas 3 opcoes

<ol>
<li>Podes copiar o codigo e editar local caso tenha o vscode</li>
<li>Podes clicar no icone do lapis para editar o codigo online</li>
<li>Podes com o codigo aberto apertar . que abrira o editor online</li>
</ol>

## 1. Remover o Alerta Inicial
No código fornecido, há um alert dentro da tag ```<script>``` que exibe a mensagem "Bem Vindo!" quando a página é carregada.
Tarefa: Remover esse alert do código.

```html
    <script>
        alert("Bem Vindo!")
    </script>
```


## 2. Adicionar Função JavaScript
No comentário fornecido, há uma instrução para copiar e colar uma função JavaScript dentro das tags ```<script>```.
Tarefa: Copiar a função minhaFuncao e colá-la dentro das tags ```<script>``` conforme a instrução abaixo.

```html
<script>
function minhaFuncao(numero) {
    const divs = document.querySelectorAll('.info-trofeu');
    divs.forEach((div, index) => {
        div.style.display = (index === numero - 1) ? 'block' : 'none';
    });
}
</script>
```

## 3. Adicionar Evento onclick nas Tags List Items ```<li>```
Adicionar um evento onclick para chamar a função minhaFuncao( N ) em cada item da lista ```<li>```, seguindo a ordem numérica (1, 2, 3, ...).

Tarefa: Adicionar onclick="minhaFuncao(número)" a cada ```<li>```, onde número corresponde à ordem do item na lista.

```html
<li onclick="minhaFuncao(1)">
    <img src="https://files.app.fcporto.pt/images/5c912fe583eeer39oPogJAJb1T9ua.jpg"><span class="number">19</span>
    <div>Taça de Portugal</div>
</li>
<li onclick="minhaFuncao(2)">
    <img src="https://files.app.fcporto.pt/images/63d80ca1b3628RrQciU9ImlRZqjlR.png"><span class="number">1</span>
    <div>Taça da Liga</div>
</li>
<li onclick="minhaFuncao(3)">
    <img src="https://files.app.fcporto.pt/images/5c9133613686ahe1ed39G3fbvocUY.jpg"><span class="number">23</span>
    <div>Supertaça</div>
</li>
```

Continue adicionando onclick nos demais ```<li>``` seguindo a ordem numérica.
