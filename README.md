# Projeto Jogo de Advinhar Número

## Pensando como um programador

Uma das coisas mais difíceis de aprender na programação não é a sintaxe que você precisa aprender, mas como aplicá-la para resolver problemas do mundo real. Você precisa começar a pensar como um programador - isso geralmente envolve olhar para as descrições do que seu programa precisa fazer e analisar como eles podem ser aplicados na solução real (prática), quais recursos de código são necessários para alcançar esse objetivo, e como fazê-los trabalhar em conjunto.

Isso requer um mistura de trabalho duro, experiência com a sintaxe de programação utilizada e prática, além de um pouco de criatividade, é claro. Quanto mais você programa, melhor programador se torna.

### O projeto chegou dessa maneira:

Quero um jogo simples de advinhar um número. O jogo deve gerar um número aleatório entre 1 e 100. O jogador terá que digitar algum número e tentar advinhar qual foi o número gerado, e isso em 10 rodadas.
A cada rodada, a aplicação terá que mostrar ao usuário os números que ele digitou, alem de mostrar se ele está certo ou errado. Caso esteja errado, mostrar se o palpite dele foi mais alto ou mais baixo do número escolhido pelo sistema.
O usuário tem que ficar ciente das vezes que ele tentou, dos número que digitou e a dica de proximidadde. 
Por fim, o usuário terá que ter a opção de jogar novamente.


### Mente programadora

Primeiro, vamos fazer uma abstração para que, em pequenas tarefas, fique realmente contextualizado para aplicarmos os códigos.

Portanto, segue o algoritmo:

```
1. Gerar um número aleatório entre 1 e 100.
2. Gravar o número do turno que o jogador está. Iniciar em 1.
3. Dar ao jogador uma forma de adivinhar o número.
4. Após a tentativa ter sido submetida, primeiro gravar em algum lugar para que o usuário possa ver as tentativas anteriores.
5. Depois, verificar se o palpite está correto.
6. Se estiver correto:
    + Escrever mensagem de parabéns.
    + Impedir que o jogador insira mais respostas (isso pode bugar o jogo).
    + Mostrar controle que permita ao jogador reiniciar o jogo.
7. Se o palpite estiver errado e o jogador ainda tem turnos sobrando:
    + Dizer ao jogador que ele está errado.
    + Permitir que ele insira outra resposta.
    + Incrementar o número do turno em 1.
8. Se o jogador está errado mas não tem turnos sobrando:
    + Dizer ao jogador que o jogo acabou.
    + Impedir que o jogador insira mais respostas (isso pode bugar o jogo).
    + Mostrar controle que permita ao jogador reiniciar o jogo.
9. Quando reiniciar, tenha certeza de resetar todas as variáveis e a interface do jogo, então volte para o passo 1.
```

### Design e Tipografia

#### Paleta de cores

#e8d5b7
#0e2430
#fc3a51
#f5b349
#e8d5b9

