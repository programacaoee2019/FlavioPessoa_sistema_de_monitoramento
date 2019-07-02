# Descrição: Programa em labview para controlar um sistema de monitoramento.

# Motivação:

Suprir a necessidade de monitorar desde a atividade de fábricas para controle de segurança e garantia de bom funcionamento a outros inúmeros sistemas que possuam alvos não fixos que precisem de monitoramento.

# Função:

Labview será utilizado para controlar o NI myRIO. Uma webcam conectada ao myRIO através de um flash drive USB realizará a captura da imagem, onde, ao detectar mudança na posição do objeto desejado, o myRIO acionará o servo para rotacionar a webcam e continuar capturando a imagem do objeto.

# Interface e utilização:

O esboço da interface é o seguinte:
![](Imagens/prototipointerface.png)

Para a utilização:

1º - Conectar o servo motor de "pan" na parte A e o servo motor de "tilt" na parte B, de acordo com a ilustração:
![](Imagens/Demo_setup_for_servo.jpg)
2º - Rodar as VIs servos.vi e Object Tracking V2.vi.  
3º - Clicar em Capturar frame.  
4º - Utilizando as formas geométricas de seleção na tela "snap image" selecionar a imagem a ser monitorada.  
5º - Com a área selecionada, clicar em selecionar objeto, que poderá ser visto na tela "template".  
6º - Ao clicar em acompanhar, a identificação começará e de acordo com a posição X do objeto, a camera será rotacionada para centralizar o objeto no centro da tela.  

Detalhes importantes:

I) A "torre" utilizada para o suporte da câmera foi a seguinte:
![](Imagens/torre.jpeg)
II) Para melhor eficiência de campo de visão, a torre deve ser posicionada com sua base(parte fixa) virada para cima.
III)A detecção da imagem fica melhor se a proporção do padrão que deve ser acompanhado se manter em escala(distância fixa da câmera).

# Recursos de terceiros utilizados

A partir do algorítimo obtido no tópico do fórum do NI de identificação de padrões na imagem da câmera desenvolvido pelo usuário Brandon L. foi possível captar os dados e a imagem para a operação dos servos motores.
link do tópico:
https://forums.ni.com/t5/Example-Programs/Object-Tracking-using-LabVIEW-and-Vision-Development-Module/ta-p/3505034?profile.language=pt-br