# Editor-de-Texto-VI
Projeto que demonstra como usar o Editor de Textos Vi / Vim (Visual Editor) do Linux

## VI e VIM
O VIM (VI improved) é um VI melhorado

## Comandos
* ':q' para sair do documento
* ':q!' saida forçada do documento
* ':wq' salva e sai do documento

## Modos
 1. Modo de Comandos (modo normal): nesse modo, as teclas não são interpretadas como caracteres, mas sim como COMANDOS
 2. Modo de Inserção (tecla 'i' para entrar e 'ESC' para sair desse modo)

## Modo de Comandos
### Para movimentação do cursor:
* 'w' e 'b' são para movimentar o cursor, são mais rápidos porque o passo é uma palavra. O comando 'w' movimenta uma pra frente e o 'b' movimenta uma palavra para trás 
* 'H' (maiúsculo) e 'L' (maiúsculo) são para movimentar o cursor, o 'H' movimento para o topo da tela (e não do arquivo) e 'L' para o final da tela
* 'G' (maiúsculo) move o cursor para o final do arquivo. Na verdade, você pode ir para quaquer linha com o comando 'xG'. Exemplo: '3G' movimenta o cursor para a linha 3. Então, para você ir para o início do documento, o comando para isso é '1G'
* '^' e '$' movem o cursor para o início da linha e para o final da linha, respectivamente. Ou seja, você pode usar expressões regulares aqui.
### Comandos importantes:
* 'r': substitui um caractere de acordo com a posição do cursor. Ex: O comando 'r7' substitui o caractere onde o cursor está apontado pelo '7'. Podemos substituir mais de uma caracter de uma vez, ex: O comando '4r!' substui os próximos 4 caracteres por '!'
* ':set number' ativa a numeração de linhas. ':set nonumber' para desativar
* O comando 'Ctrl + g' mostra a quantidade total de linhas do documento
* O comando 'a' é usado para adicionar um texto a partir da posição seguinte do cursor 
* ~ : muda o case do caractere, exemplo: Se o cursor está no início dessa linha 'acid' e o comando '4~' for selecionado, o resultado vai ser a linha com 'ACID'
* 'J' (maiúsculo): junta duas linhas
* 'x': apaga o caractere em que está o cursor, vale lembra que você pode especificar quantos caracteres irão ser apagados
* 'u': comando que desfaz a última operação e o 'Ctrl R' que refaz a última operação. Com esses dois comandos, você pode desempilhar e empilhar a pilha de alteração do documento
* Para buscar uma palavra no Vi/Vim, basta digitar '/' seguido da palavra para fazer a pesquisa
### Copiar, colar e recortar:
* 'yy': copia a linha inteira. Você pode especificar a quantidade de linhas copiadas, por exemplo, o comando 'y3' copia a linha atual e as próximas 3
* 'yw': copia a palavra inteira
* 'p': cola
* 'dd': recorta a linha atual inteira. O comando '3dd' recorta 3 linhas a partir da linha atual do cursor
* 'dw': recorta a palavra atual de onde está o cursor
