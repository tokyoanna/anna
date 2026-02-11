1. O que é o Node.js?

O Node.js é um ambiente de execução que permite rodar código JavaScript fora do navegador, geralmente no servidor.

Ele não é uma linguagem de programação porque não cria uma nova sintaxe ou linguagem. Ele apenas executa JavaScript, utilizando o motor V8 do Google Chrome.

Sua principal finalidade é permitir a criação de aplicações back-end, como servidores web, APIs, sistemas em tempo real e automações.

2. Diferença entre Node.js e JavaScript no navegador

1ª Diferença – Ambiente de execução:

No navegador, o JavaScript roda no cliente (front-end).

No Node.js, o JavaScript roda no servidor (back-end).

2ª Diferença – APIs disponíveis:

No navegador, temos acesso ao DOM (document, window, etc.).

No Node.js, não existe DOM, mas existem APIs para acessar arquivos, sistema operacional, rede, banco de dados, etc.

3. O que é o V8 Engine?

O V8 Engine é o motor de JavaScript criado pelo Google para o Chrome.

Sua importância para o Node.js é que ele:

Interpreta e executa o código JavaScript.

Compila JavaScript em código de máquina, tornando a execução mais rápida.

Sem o V8, o Node.js não conseguiria executar JavaScript.

4. O que é I/O não bloqueante?

I/O (Input/Output) não bloqueante significa que o Node.js não precisa esperar uma operação terminar (como leitura de arquivo ou requisição ao banco) para continuar executando o restante do código.

Exemplo:

Enquanto um arquivo está sendo lido, o servidor pode continuar atendendo outras requisições.

Isso melhora o desempenho porque:

Evita que o sistema fique “travado”.

Permite atender muitas conexões simultaneamente.

Torna aplicações mais rápidas e escaláveis.

5. O que é o Event Loop?

O Event Loop é o mecanismo que permite ao Node.js executar operações assíncronas.

Funcionamento resumido:

O código é executado.

Operações demoradas (I/O) são enviadas para o sistema.

Quando terminam, elas entram em uma fila.

O Event Loop verifica constantemente essa fila e executa as funções de retorno (callbacks).

Ele é o responsável pelo funcionamento assíncrono do Node.js.

6. O que são módulos no Node.js?

Módulos são blocos de código reutilizáveis que podem ser importados em outros arquivos.

Tipos:

🔹 Módulos internos (core modules)
Já vêm com o Node.js.
Ex: fs, http, path.

🔹 Módulos externos
São instalados via npm.
Ex: express, axios.

🔹 Módulos criados pelo desenvolvedor
Arquivos criados no próprio projeto e exportados com module.exports.

7. Para que serve o package.json?

O package.json é o arquivo que gerencia as informações do projeto.

Ele pode conter:

Nome e versão do projeto

Lista de dependências

Scripts (ex: "start": "node index.js")

Autor

Licença

Descrição

8. O que é o npm?

O npm (Node Package Manager) é o gerenciador de pacotes do Node.js.

Funções principais:

Instalar bibliotecas

Gerenciar dependências

Atualizar pacotes

Executar scripts do projeto

Ele facilita o reaproveitamento de código e acelera o desenvolvimento.

9. O que é uma API REST?

Uma API REST é uma interface que permite comunicação entre sistemas através do protocolo HTTP, utilizando métodos como:

GET

POST

PUT

DELETE

O Node.js pode ser usado para criar APIs REST utilizando frameworks como Express, permitindo:

Criar rotas

Receber requisições

Enviar respostas em JSON

Conectar com bancos de dados

10. Vantagens e desvantagens do Node.js

Vantagens:

Alto desempenho (I/O não bloqueante).

Usa JavaScript no front-end e no back-end (mesma linguagem).

Desvantagens:

Não é ideal para tarefas muito pesadas de CPU.

Código assíncrono pode ficar complexo (callback hell, se mal estruturado).
