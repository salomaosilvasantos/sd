### Pr�tica de Blockchain

- Neste trabalho foi utilizado blockchain para simular o registro de votos de uma elei��o para presidente de um pa�s. 

- Para este trabalho, foi utilizado uma estrutura de blocos em cadeia, de modo que cada voto da elei��o � representado por um bloco.  A estrutura do bloco �:

 > id: identificador do voto
 > data : representa os dado do voto, constitu�do por data, hora e nomo do presidente votado.
 > hash: c�digo do hash do voto atual :
 > previousHash: c�digo do hash do voto anterior :

- Os blocos gerados s�o salvos em um arquivo JSON. Depois, os blocos s�o lidos do arquivo JSON e validados.

- Na conhecimento adiquirido sobre blockchain, foi poss�vel observar que para v�lidar uma cadeia deve-se verificar, se o ultimo bloco esta v�lido. Ou seja, se ao gerar seu hash, foi utilizado o hash do anterior e assim sucessivamente. Essa verifica��o � feita em todos os blocos da cadeia, at� que todos seja considerados v�lidos.