# Descri��o: Programa em labview para controlar um sistema de monitoramento.

# Motiva��o:

Suprir a necessidade de monitorar desde a atividade de f�bricas para controle de seguran�a e garantia de bom funcionamento a outros in�meros sistemas que possuam alvos n�o fixos que precisem de monitoramento.

# Fun��o:

Labview ser� utilizado para controlar o NI myRIO. Uma webcam conectada ao myRIO atrav�s de um flash drive USB realizar� a captura da imagem, onde, ao detectar mudan�a na posi��o do objeto desejado, o myRIO acionar� o servo para rotacionar a webcam e continuar capturando a imagem do objeto.

# Interface e utiliza��o:

O esbo�o da interface � o seguinte:
![](Imagens/prototipointerface.png)

Para a utiliza��o:

1� - Rodar a VI.  
2� - Clicar em Capturar frame.  
3� - Utilizando as formas geom�tricas de sele��o na tela "snap image" selecionar a imagem a ser monitorada.  
4� - Com a �rea selecionada, clicar em selecionar objeto, que poder� ser visto na tela "template".  
5� - Ao clicar em acompanhar, a identifica��o come�ar� e de acordo com a posi��o X do objeto, a camera ser� rotacionada para centralizar o objeto no centro da tela.  