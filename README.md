https://www.yunguerdvorak.com/projetos/chess-c/

programar um jogo de xadrez em C, uma abordagem comum para representar o tabuleiro é usar uma matriz bidimensional de 8x8. Esta matriz reflete a organização visual do tabuleiro, onde cada célula pode armazenar informações sobre a peça que ocupa aquela casa. 
Elaboração:
Representação do Tabuleiro:
Uma matriz tabuleiro[8][8] pode ser usada para representar o tabuleiro, onde cada elemento da matriz corresponde a uma casa no tabuleiro. 
Armazenamento de Informações:
Cada elemento da matriz pode conter informações sobre a peça que ocupa aquela casa, como tipo de peça (peão, torre, cavalo, etc.), cor (branca ou preta), e, possivelmente, outras informações relevantes para a jogabilidade. 
Movimento das Peças:
Para implementar a movimentação das peças, você pode usar as coordenadas da matriz (índices) para identificar a casa de origem e destino da peça. A validação dos movimentos pode ser feita através de regras específicas para cada peça, como a movimentação diagonal do bispo ou a movimentação em "L" do cavalo. 
Validação de Movimentos:
É importante validar se um movimento é válido antes de permitir que seja realizado. Isso envolve verificar se o movimento está dentro das regras do jogo, se há alguma peça no caminho (para peças como torre, bispo, e dama), e se o movimento coloca o rei do jogador em xeque. 
Captura de Peças:
Quando uma peça se move para uma casa ocupada por uma peça do adversário, a peça capturada é removida do tabuleiro, e a peça que se move assume a posição da casa. 
Xeque e Xeque-Mate:
A lógica do jogo deve incluir a detecção de xeque (quando o rei está sob ataque) e xeque-mate (quando o rei está em xeque e não há movimentos legais para se defender). 
Interface com o Usuário:
Para permitir que os jogadores interajam com o jogo, você pode criar uma interface gráfica (se você tiver uma biblioteca gráfica em C, como SDL ou OpenGL) ou uma interface de texto para exibir o tabuleiro, solicitar as jogadas, e mostrar