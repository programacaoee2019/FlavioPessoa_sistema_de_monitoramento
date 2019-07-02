# Descri��o: Programa em labview para controlar um sistema de monitoramento.

# Motiva��o:

Suprir a necessidade de monitorar desde a atividade de f�bricas para controle de seguran�a e garantia de bom funcionamento a outros in�meros sistemas que possuam alvos n�o fixos que precisem de monitoramento.

# Fun��o:

Labview ser� utilizado para controlar o NI myRIO. Uma webcam conectada ao myRIO atrav�s de um flash drive USB realizar� a captura da imagem, onde, ao detectar mudan�a na posi��o do objeto desejado, o myRIO acionar� o servo para rotacionar a webcam e continuar capturando a imagem do objeto.

# Interface e utiliza��o:

O esbo�o da interface � o seguinte:
![](Imagens/prototipointerface.png)

Para a utiliza��o:

1� - Conectar o servo motor de "pan" na parte A e o servo motor de "tilt" na parte B, de acordo com a ilustra��o:
![](Imagens/Demo_setup_for_servo.jpg)
2� - Rodar as VIs servos.vi e Object Tracking V2.vi.  
3� - Clicar em Capturar frame.  
4� - Utilizando as formas geom�tricas de sele��o na tela "snap image" selecionar a imagem a ser monitorada.  
5� - Com a �rea selecionada, clicar em selecionar objeto, que poder� ser visto na tela "template".  
6� - Ao clicar em acompanhar, a identifica��o come�ar� e de acordo com a posi��o X do objeto, a camera ser� rotacionada para centralizar o objeto no centro da tela.  

Detalhes importantes:

I) A "torre" utilizada para o suporte da c�mera foi a seguinte:
![](Imagens/torre.jpeg)
II) Para melhor efici�ncia de campo de vis�o, a torre deve ser posicionada com sua base(parte fixa) virada para cima.
III)A detec��o da imagem fica melhor se a propor��o do padr�o que deve ser acompanhado se manter em escala(dist�ncia fixa da c�mera).

# Recursos de terceiros utilizados

A partir do algor�timo obtido no t�pico do f�rum do NI de identifica��o de padr�es na imagem da c�mera desenvolvido pelo usu�rio Brandon L. foi poss�vel captar os dados e a imagem para a opera��o dos servos motores.
link do t�pico:
https://forums.ni.com/t5/Example-Programs/Object-Tracking-using-LabVIEW-and-Vision-Development-Module/ta-p/3505034?profile.language=pt-br