# ActionScript
Isabelly Thayse Araújo Alves - IsabellyAraujo - 20141011110077 <br>
Lara Costa Belarmino de Macêdo - larabelarmino - 20151011110392 <br>
Amanda Alves da Silva - amandaalves -  20141011110093 

## Resumo

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
 
 * **Uso** <br>
  Abra o Flash, clique em File > New, selecione o Arquivo ActionScript e clique em Ok. Uma caixa de diálogo irá se abrir, agora siga os passos abaixo para compilar o seu código.
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
               hello.text = "Hello world!";
               hello.x = 100;
               hello.y = 100;
               addChild(hello);
           }
       }   

   <br>**2.** Abra o prompt, vá até a pasta onde você salvou o arquivo acima e digite:
     >>
        $ mxmlc nomedoarquivo.as

    <br>**3.** Após a compilação, confira se existe um arquivo .swf com o mesmo nome do arquivo .as que já foi salvo.
    
    <br>**4.**  clique em Arquivo, depois Abrir e selecione o arquivo .swf desejado.
    
    
### Sintaxe Básica

 >### Variáveis e constantes
  >>Tipos aceitos:
  >>>String
  >>>Int
  >>>Boolean
  >>>Number
  >>>Object
  >>>Class
  >>>Array
  
  >>Declarando
  ~~~
  var myPhoneNumper: Number;
  ~~~

>### Operadores Relacionais e Lógicos
 >> >
 >> <
 >> =>
 >> <=
 >> ==
 >> !=
 >> &&
 >> ||
 >> ++
 >> --

>### Operadores Aritméticos
>> #### +
>> #### -
>> #### *
>> #### /

>>Exemplo:
~~~
var numer1:int = 2 * 3 + 1 / 2 - 1;
~~~

>### Estruturas de Controle Condicional

>> ### Switch

>>>Exemplo:
~~~
switch (myVariable)
{
	case 1:
	statements;
	break;
}
~~~

>> ### If
>>>Exemplo:
~~~
if(condition){
	statements;
}
~~~

~~~
var idade:Number = 20;
if(idade >  18){
	trace("Bem-vindo(a)!");
}
~~~

>>### Else/Else if
>>>Exemplo:
~~~
var idade:Number = 20;
if(idade > 18){
	trade("Bem-Vindo(a)!");
}
else if(idade < 18){
	trade("Ops, você não deve estar aqui");
}
else 
	trade("Forbidden");
~~~

>### Estruturas de Repetição

>> ### While
>>>Exemplo:
~~~
var i:Number = 0;
while(i < 10){
	trade(i);
	i++;
}
~~~

>> ### Do While
>>>Exemplo:
~~~
var i:Number = 0;
do{
	trade(i);
	i++;
} while (i < 10);
~~~

>> ### For

>>>Exemplo:
~~~
for(var i:Number=0; i<10; i++){
	trace(i);
}
~~~

>> ### Foreach
>>>Exemplo:
~~~
	var obj:Object = new objeto();
	obj.i = "Olá";
	obj.n = 12;
	foreach(var f in obj)
	{
		trace(f);
	}
~~~
>> ### For In
>>>Exemplo:
~~~
var obj.Object = new objeto();
obj.i = "Olá!";
obj.n = 12;
for (var f in obj){
	trace(f);
}
~~~

>> ### Vetores, matrizes e strings

>>> ### String: Substring
>>>Exemplo:
~~~
var str:String = "Hello from Paris, Texas!!!";
trace(str.substr(11,15)); //output: Paris, Texas!!!
trace(str.substring(11,15)); //output: Pari 
~~~

>>> ### String: Upper/Lower Case
>>>Exemplo:
~~~
var str:String = "Dr. Bob Roberts, #9."
trace(str.toLowerCase()); //dr. bob roberts, #9.
trace(str.toUpperCase()); //DR. BOB ROBERTS, #9.
~~~

>>> ### String: Sort
>>>Exemplo:
~~~
var str:String = "hello world!";
for (var i:int = 0; i < str.lengh; i++)
{
	trace(str.charAt(i), "-", str.charCodeAt(i));
}
~~~

>>> ### Array

>>>Exemplo:

~~~
var myArray:Array = ["Flash", "ActionScript"];
~~~

>> ### Funções

>>> ### Funções Básicas
>>>Exemplo:
~~~
function Nome_Funcao(argumento):returnType{
	statements;
}
~~~

## Sintaxe OO

### Classes
* Sintaxe para definição de uma classe:<br>
~~~
class nome_da_classe_sem_espacos{
//corpo da classe
}
~~~
**Exemplo:**<br>
~~~
class carro
{
public var placa:String = “MM 0056”;
private var volume_tanque:Number = 30;

public function acender_farol(){
return 1;
}

private var queimar_gasolina(){
return 1;
}
static function getNumeroRodas(){
return 4;
}
}
~~~

### Objetos

* Sintaxe para criação (instanciação) de um objeto:<br>
~~~
var nomeDoObjeto = new nomeDaClasse();
~~~

### Atributos (visibilidade: privado e público, escopo: classe e objeto)
|  Atributo | Definição |
| --- | --- |
| dinâmico | Permitir que propriedades sejam adicionadas a ocorrências em tempo de execução. |
|final | Não deve ser estendido por outra classe. |
| internal (padrão)| Visível para referências dentro do pacote atual.|
| public | Visível para referências em todos os lugares. |
### Métodos (visibilidade: privado e público, escopo: classe e objeto)


### Métodos (visibilidade: privado e público, escopo: classe e objeto)

### Construtores

### Herança

### Polimorfismo

### Sobrecarga

### Exceções

#### Categorias de exeções

#### Captura e lançamento de exceções

#### Criar novas exeções
