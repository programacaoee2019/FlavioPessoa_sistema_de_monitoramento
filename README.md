# Descrição: Programa em labview para controlar um sistema de monitoramento.

# Motivação:

Suprir a necessidade de monitorar desde a atividade de fábricas para controle de segurança e garantia de bom funcionamento a outros inúmeros sistemas que possuam alvos não fixos que precisem de monitoramento.

# Função:

Labview será utilizado para controlar o NI myRIO. Uma webcam conectada ao myRIO através de um flash drive USB realizará a captura da imagem, onde, ao detectar mudança na posição do objeto desejado, o myRIO acionará o servo para rotacionar a webcam e continuar capturando a imagem do objeto.

# Interface e utilização:

O esboço da interface é o seguinte:
![](Imagens/prototipointerface.png)

Para a utilização:

1º - Rodar a VI.  
2º - Clicar em Capturar frame.  
3º - Utilizando as formas geométricas de seleção na tela "snap image" selecionar a imagem a ser monitorada.  
4º - Com a área selecionada, clicar em selecionar objeto, que poderá ser visto na tela "template".  
5º - Ao clicar em acompanhar, a identificação começará e de acordo com a posição X do objeto, a camera será rotacionada para centralizar o objeto no centro da tela.  