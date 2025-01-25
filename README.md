README - Sistema de Sorteio de Amigo Secreto

Sobre o Projeto

Este é um projeto simples para gerenciar e sortear nomes para um amigo secreto. Ele permite que os usuários:

Adicionem nomes à lista de participantes.

Visualizem a lista de participantes na página.

Realizem o sorteio de um participante aleatoriamente.

Funcionalidades

1. Adicionar Amigos

Campo de entrada para digitar o nome do participante.

Os nomes são armazenados em uma lista interna e exibidos em uma lista na interface do usuário.

Caso o nome não seja informado, o sistema exibe um alerta solicitando o preenchimento.

2. Realizar Sorteio

Realiza um sorteio aleatório entre os nomes cadastrados.

Caso a lista esteja vazia, exibe um alerta informando que é necessário adicionar participantes.

Exibe o nome sorteado na interface do usuário.

Como Usar

Adicionar um Nome à Lista

Digite o nome de um participante no campo de texto.

Clique no botão correspondente para adicionar o nome à lista.

Realizar o Sorteio

Após adicionar os nomes, clique no botão de sorteio.

O nome sorteado será exibido na área destinada ao resultado.

Estrutura do Código

Seleção de Elementos do HTML

inputAmigo: Campo de texto onde o usuário insere o nome do participante.

listaAmigos: Lista visual onde os nomes são exibidos.

resultado: Local onde o nome sorteado é exibido.

Lógica do Programa

Lista de Participantes

Os nomes dos participantes são armazenados no array nomes, que é utilizado para gerenciar as informações internamente.

Funções

adicionarAmigo

Adiciona o nome digitado pelo usuário à lista de participantes.

Valida se o campo não está vazio antes de adicionar o nome.

Atualiza a interface exibindo o nome na lista visível.

sortearAmigo

Verifica se a lista possui participantes antes de realizar o sorteio.

Seleciona aleatoriamente um nome da lista.

Exibe o nome sorteado na interface.

Requisitos

Navegador com suporte a JavaScript.

HTML com os seguintes elementos:

Campo de entrada com id="amigo".

Lista de itens com id="listaAmigos".

Elemento para exibir o resultado com id="resultado".

Observações

Este código é uma aplicação simples e pode ser expandida com recursos adicionais, como remoção de nomes, estilização personalizada ou persistência de dados.

Sempre teste o sistema em diferentes navegadores para garantir a compatibilidade.

Exemplo de Uso

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Amigo Secreto</title>
</head>
<body>
    <input id="amigo" type="text" placeholder="Digite o nome">
    <button onclick="adicionarAmigo()">Adicionar</button>
    <ul id="listaAmigos"></ul>
    <button onclick="sortearAmigo()">Sortear</button>
    <p id="resultado"></p>
</body>
<script src="script.js"></script>
</html>

Licença

Este projeto é de uso livre e pode ser adaptado conforme necessário.
