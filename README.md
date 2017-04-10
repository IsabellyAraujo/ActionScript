# ActionScript
Isabelly Thayse Araújo Alves - IsabellyAraujo - 20141011110077 <br>
Lara Costa Belarmino de Macêdo - larabelarmino - 20151011110392 <br>
Amanda Alves da Silva - amandaalves -  20141011110093 

## Resumo

A ActionScript é uma linguagem de script orientada a objetos baseada no ECMAScript (linguagem de programação baseada em scripts), utilizada principalmente para construção de aplicações RIA (Rich Internet Applications, traduzindo, Aplicações Ricas de Internet, como o Flicker, Gmail, Pixlr). É executada em uma máquina virtual (AVM - "ActionScript Virtual Machine"), atualmente na versão 3 que está disponível no Adobe Flash Player (plug-in encontrado em navegadores web) e também no ambiente Adobe AIR.
<br>
A ActionScript foi criada por Gary Grossman, em 1998, e desenvolvida pela Macromedia, hoje controlada pela Adobe. A linguagem foi influenciada pelas linguagens Java e Javascript, podendo ser compilada em Flash e Adobe Flex.
 ## Instalação e uso
 
  *  **Instalação** <br>
  
 Como sabemos, A ActionScript é a linguagem de criação de scripts do Adobe Flash, que já vem instalado com ela. Para executar a instalação, siga as instruções a seguir:<br>
  1. Você precisa ter o arquivo .exe do Adobe Flash baixado em seu computador para poder iniciar a instalação;<br>
  2. Execute o Instalador.  Em seguida, clique em “sim”. Caso seja necessário autorizar a instalação, insira o usuário e a senha de um administrador;<br>
 3. Escolha a forma que deseja receber as atualizações do programa e, em seguida, clique em “próximo”;<br>
 4. Aguarde a conclusão do download e a instalação;<br>
 5. Clique em concluir. 
 
 * **Uso**
   * Compilando<br>
   
    **1.** Escreva o código e salve o arquivo.<br>
    
      * Exemplo:<br>
      
    >> 
         package {
          import flash.display.Sprite;
          import flash.text.TextField;

          public class Hello extends Sprite{

           [SWF(width="500", height="500")]
           public function Hello () {
               var hello:TextField = new TextField();
               t.text = "Hello world!";
               t.x = 100;
               t.y = 100;
               addChild(hello);
           }
       }   

   <br>**2.** Abra o prompt, vá até a pasta que você salvou o arquivo acima e digite:
     >>
        $ mxmlc nomedoarquivo.as

