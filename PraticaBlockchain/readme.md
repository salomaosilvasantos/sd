### Pr�tica de Blockchain

- Neste trabalho foi utilizado *blockchain* para simular o registro de votos de uma elei��o para presidente de um pa�s. 

- Para este trabalho, foi utilizado uma estrutura de blocos em cadeia, de modo que cada resgistro de voto da elei��o � representado por um bloco.  A estrutura do bloco �:

            > id: identificador do voto.
            > data : representa os dados do voto, constitu�do por data, hora e nomo do presidente votado.
            > hash: c�digo do hash do voto atual.
            > previousHash: c�digo do hash do voto anterior.

- Os blocos gerados s�o salvos em um arquivo JSON. Depois, os blocos s�o lidos do arquivo JSON e validados.


- No conhecimento adiquirido sobre *blockchain*, existem dois tipos b�sicos de registros: *blocos e transa��es*. Come�ando com um bloco inicial(chamado de bloco g�nese) que registra o estado inicial do banco de dados, seguido pelos blocos subsequentes, cada qual cont�m, um grupo de transa��es j� validadas. Cada bloco da cadeia, exceto o g�nese, cont�m um hash do bloco anterior, criando um encadeamento entre eles e garantindo a integridade da informa��o, j� que � impossivel alterar blocos antigos sem alterar todos os blocos subsequentes. Portanto, pode-se entender um blockchain como um estado inicial seguido de um certo n�mero de fun��es de transi��o, agrupados em blocos. De fato, o estado atual do banco de dados est� contido em um blockchain apenas de maneira abstrata, sendo necess�rio que cada n� determine tal estado partindo do inicial e aplicando as subsequentes transa��es.