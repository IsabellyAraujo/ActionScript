# ActionScript
Isabelly Thayse Araújo Alves - IsabellyAraujo - 20141011110077 <br>
Lara Costa Belarmino de Macêdo - larabelarmino - 20151011110392 <br>
Amanda Alves da Silva - amandaalves -  20141011110093 

## Resumo

<br>
A linguagem ActionScript foi criada por Gary Grossman, em 1998, e desenvolvida pela Macromedia, hoje controlada pela Adobe. A ActionScript é uma linguagem multiparadigmal de script baseada no ECMAScript, assim como a JavaScript, utilizada principalmente para construção de aplicações RIA (Aplicações Ricas de Internet), como o Flickr e o Deezer.
É executada em uma máquina virtual (AVM - "ActionScript Virtual Machine"), atualmente na versão 3.0 que está disponível no Adobe Flash Player (plug-in encontrado em navegadores web) e também no ambiente Adobe AIR. 
Seu estilo de tipagem é estática, forte e robusta. O que implica em dizer que sua tipagem é conhecida durante a compilação e  os objetos/variáveis tem um tipo bem definido e que precisa ser informado no momento de sua declaração, além de ser possível identificar os erros pelas stack traces durante a compilação, etc.

## Instalação e Uso
 
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
  >>Variáveis: 
  >>>String<br>
  >>>Number<br>
  >>>Int<br>
  >>>Uint<br>
  >>>Boolean<br>
  >>>Object<br>
  >>>Class<br>
  >>>Date<br>
  >>>Array<br>
  
  >Declarando
  ~~~
  var myPhoneNumper: Number;
  ~~~

 >>Constantes:
 >Declarando:
 ~~~
 const taxa_desconto:Number = 0.07;
 ~~~
 
>### Operadores Relacionais e Lógicos
 >>Relacionais:<br>
 >>>**>**<br>
 >>> **<**<br>
 >>> **=>**<br>
 >>> **<=**<br>
 >>> **==**<br>
 >>> **!=**<br>
 
 >>Lógicos:<br>
 >>> **&&**<br>
 >>> **||**<br>

>### Operadores Aritméticos
>> #### +
>> #### -
>> #### *
>> #### /
>> #### %

>Exemplo:
~~~
var numer1:Int = 2 * 3 + 1 / 2 - 1;
~~~

>### Estruturas de Controle Condicional

>> ### Switch

>Exemplo:<br>
~~~
switch (myVariable)
{
	case 1:
	statements;
	break;
}
~~~

>> ### If
>Exemplo:
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
>Exemplo:
~~~
var idade:Number = 20;
if(idade > 18){
        trace("Bem-Vindo(a)!");
}
else if(idade < 18){
        trace("Ops, você não deve estar aqui");
}
else 
        trace("Forbidden");
~~~

>### Estruturas de Repetição

>> ### While
>Exemplo:
~~~
var i:Number = 0;
while(i < 10){
	trace(i);
	i++;
}
~~~

>> ### Do While
>Exemplo:
~~~
var i:Number = 0;
do{
	trace(i);
	i++;
} while (i < 10);
~~~

>> ### For

>Exemplo:
~~~
for(var i:Number=0; i<10; i++){
	trace(i);
}
~~~

>> ### Foreach
>Exemplo:
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
>Exemplo:
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
>Exemplo:
~~~
var str:String = "Hello from Paris, Texas!!!";
trace(str.substr(11,15)); //output: Paris, Texas!!!
trace(str.substring(11,15)); //output: Pari 
~~~

>>> ### String: Upper/Lower Case
>Exemplo:
~~~
var str:String = "Dr. Bob Roberts, #9."
trace(str.toLowerCase()); //dr. bob roberts, #9.
trace(str.toUpperCase()); //DR. BOB ROBERTS, #9.
~~~

>>> ### String: Sort
>Exemplo:
~~~
var str:String = "hello world!";
for (var i:int = 0; i < str.lengh; i++)
{
	trace(str.charAt(i), "-", str.charCodeAt(i));
}
~~~

>>> ### Substring
>Exemplo:
~~~
var str:String = "Hello from Paris, Texas!!!";
trace(str.slice(11,15)); // output: Pari
trace(str.slice(-3,-1)); // output: !!
trace(str.slice(-3,26)); // output: !!!
trace(str.slice(-3,str.length)); // output: !!!
trace(str.slice(-8,-3)); // output: Texas
~~~

>>> ### Concatenação
>Exemplo: 
~~~
var str1:String = "green";
var str2:String = "ish";
var str3:String = str1 + str2; // str3 == "greenish"
~~~

~~~
var str:String = "green";
str += "ish"; // str == "greenish"
Além disso, a classe String inclui um método concat() que pode ser usado da seguinte maneira:
var str1:String = "Bonjour";
var str2:String = "from";
var str3:String = "Paris";
var str4:String = str1.concat(" ", str2, " ", str3);
// str4 == "Bonjour from Paris"
~~~

>>> ### Array

>Exemplo:

~~~
var myArray:Array = ["Flash", "ActionScript"];
~~~

>>> ### Matrizes<br>
Matriz Multidimensional: Duas matrizes indexadas

~~~
var ListaTarefas:Array = new Array(); 
ListaTarefas[0] = ["wash dishes", "take out trash"]; 
ListaTarefas[1] = ["wash dishes", "pay bills"]; 
ListaTarefas[2] = ["wash dishes", "dentist", "wash dog"]; 
ListaTarefas[3] = ["wash dishes"]; 
ListaTarefas[4] = ["wash dishes", "clean house"]; 
ListaTarefas[5] = ["wash dishes", "wash car", "pay rent"]; 
ListaTarefas[6] = ["mow lawn", "fix chair"];
~~~

~~~
traceListaTarefas[2][1]); // output: dentist
~~~

Matriz associativa com uma matriz indexada

~~~
var ListaTarefas:Object = new Object(); 
ListaTarefas["Monday"] = ["wash dishes", "take out trash"]; 
ListaTarefas["Tuesday"] = ["wash dishes", "pay bills"]; 
ListaTarefas["Wednesday"] = ["wash dishes", "dentist", "wash dog"]; 
ListaTarefas["Thursday"] = ["wash dishes"]; 
ListaTarefas["Friday"] = ["wash dishes", "clean house"]; 
ListaTarefas["Saturday"] = ["wash dishes", "wash car", "pay rent"]; 
ListaTarefas["Sunday"] = ["mow lawn", "fix chair"];
~~~

>> ### Funções

>>> ### Funções Básicas
>Exemplo:

~~~
function Nome_Funcao(argumento):returnType{
	statements;
}
~~~

## Sintaxe OO

### Classes
* Sintaxe para definição de uma classe:<br>
~~~
public class nome_da_classe_sem_espacos{
//corpo da classe
}
~~~
**Exemplo:**<br>
~~~
public class carro
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
var nomeDoObjeto: nomeDaClasse= new nomeDaClasse();
~~~

### Atributos (visibilidade: privado e público, escopo: classe e objeto)
|  Tipo  |  Definição |
| --- | --- |
| internal (padrão) | Visível para referências dentro do mesmo pacote. |
|private | Visível para referências na mesma classe. |
|protected| Visível para referências na mesma classe e em classes derivadas.|
| public | Visível para referências em todos os lugares. |
| static | Especifica que uma propriedade pertence à classe, ao contrário das ocorrências da classe.|
| UserDefinedNamespace | Nome do espaço para nomes personalizado definido pelo usuário. |
#### Exemplo:
Private:
~~~
class PrivateExample
{
 private var privVar:String = "private variable";
}
var myExample:PrivateExample = new PrivateExample();
trace(myExample.privVar);// compile-time error in strict mode
trace(myExample["privVar"]); // ActionScript 2.0 allows access, but in ActionScript 3.0, this
is a run-time error. 
~~~

### Métodos 
Um método é uma ação que um objeto pode realizar.<br>
Abaixo, observamos exemplos de métodos que orientam o MovieClip chamado *shortFilm*.<BR>
Este método instrui o MovieClip a iniciar a reprodução:
~~~
shortFilm.play();
~~~

Este método faz o *MovieClip* parar a reprodução:
~~~
shortFilm.stop();
~~~
Este método faz o *MovieClip* mover o indicador de reprodução para o começo e parar a reprodução:
~~~
shortFilm.gotoAndStop(1);
~~~

### Construtores
O código de um método de construtor é executado toda vez que uma ocorrência da classe é criada com *new*.
Exemplo:
~~~
class Example
{
 public var status:String;
 public function Example()
 {
 status = "initialized";
 }
}
var myExample:Example = new Example();
trace(myExample.status); // output: initialized
~~~
Construtores só podem ser públicos, sendo assim opcional a utilização do atributo *public*.

### Herança e Poliformismo
É utilizada a palavra *extends* para para indicar que uma classe herda de outra classe.<br>
Na herança, pode-se usar o poliformismo do código, como no exemplo abaixo, onde, devido ao poliformismo a classe *area()* vai fazer os respectivos cálculos para os objetos do tipo *Square* e *Circle*:
~~~
class Shape 
{ 
    public function area():Number 
    { 
        return NaN; 
    } 
} 
 
class Circle extends Shape 
{ 
    private var radius:Number = 1; 
    override public function area():Number 
    { 
        return (Math.PI * (radius * radius)); 
    } 
} 
 
class Square extends Shape 
{ 
    private var side:Number = 1; 
    override public function area():Number 
    { 
        return (side * side); 
    } 
} 
 
var cir:Circle = new Circle(); 
trace(cir.area()); // output: 3.141592653589793 
var sq:Square = new Square(); 
trace(sq.area()); // output: 1
~~~
Se uma propriedade for declarada como pública, ela será visível em qualquer lugar de código. Ao contrário das propriedades declaradas como: *private, protected e internal*, a *public* não coloca nenhuma restrição sobre a herança da propriedade.

### Sobrecarga

A sobrecarga (*Overload*), métodos de mesmo nome, que tem com argumentos diferentes (seja em número e/ou tipo de dado). <BR>
O ActionScript não suporta sobrecarga.

### Exceções
O AS3 dá suporte ao tratamento de exessões através da cláusula try/catch/finally e das classes de erro.
#### Categorias de exeções

* Erros de tempo de compilação: ocorrem quando problemas sintáticos no seu código impedem a criação do aplicativo.
* Erros de tempo de execução:  ocorrem quando você executa o aplicativo depois de compilá-lo.
* Erros síncronos: são erros de tempo de execução que ocorrem no momento em que uma função é chamada.
* Errosassíncronos: são erros de tempo de execução que ocorrem em vários momentos durante o tempo de execução.
* Exceções não detectadas: são erros lançados sem nenhuma lógica correspondente (como uma instrução catch) em resposta a elas.

#### Captura e lançamento de exceções

Define-se um bloco *try* para verificar se código possui algum erro, se esse for o caso é executado o bloco contido em *catch*.<br>
Exemplo:
~~~
var MyError:Error = new Error("Encountered an error with the numUsers value", 99); 
var numUsers:uint = 0; 
try 
{ 
    if (numUsers == 0) 
    { 
        trace("numUsers equals 0"); 
    } 
} 
catch (error:uint) 
{ 
    throw MyError; // Catch unsigned integer errors. 
} 
catch (error:int) 
{ 
    throw MyError; // Catch integer errors. 
} 
catch (error:Number) 
{ 
    throw MyError; // Catch number errors. 
} 
catch (error:*) 
{ 
    throw MyError; // Catch any other error. 
} 
finally  
{ 
    myFunction(); // Perform any necessary cleanup here. 
}
~~~
A instrução *finally* delimitará as instruções que serão executadas caso ocorra ou não um erro no bloco *try*. Se não houver nenhum erro, as instruções no bloco *finally* serão executadas depois que as instruções do bloco *try* forem concluídas. Os blocos *catch* e *finally* são opcionais, porém, é preciso que um deles esteja presente; caso contrário será lançado um erro de compilação.

#### Criar novas exeções
Com o *throw*, você pode lançar erros explicitamente.<br>
Você também pode estender uma das classes Error padrão para criar suas próprias classes de erro no ActionScript, você pode usar-las para identificar erros ou grupos de erros específicos que são exclusivos do seu aplicativo ou para fornecer recursos de exibição de erros exclusivos para os erros gerados pelo seu aplicativo.<br>
Uma classe de erro especializada deve estender a classe Error principal do ActionScript. Veja um exemplo de uma classe AppError especializada que estende a classe Error:<br>
Classe:
~~~
public class AppError extends Error 
{ 
    public function AppError(message:String, errorID:int) 
    { 
        super(message, errorID); 
    } 
}
~~~
AppError no projeto:
~~~
try 
{ 
    throw new AppError("Encountered Custom AppError", 29); 
} 
catch (error:AppError) 
{ 
    trace(error.errorID + ": " + error.message) 
}
~~~

## Sintaxe Funcional
### Conceitos de funções básicas
#### Chamada de funções

Quando utilizamos o identificador de uma função seguido de parênteses, uma função é chamada.
- Exemplo:
~~~
trace()
~~~

Se uma função estiver com os parênteses vazios, significa que ela não possui um parâmetro.
- Exemplo:
~~~
var randomNum:Number = math.random()
~~~
#### Instruções de função

Para definir uma função, é necessário seguir os seguintes passos:<br>
	1) Utilizar a palavra-chave “function”;<br>
	2) Dar um nome à função;<br>
	3) Definir os parâmetros em uma lista delimitada por vírgulas e parênteses;<br>
	4) Fazer o corpo da função, que deve ficar entre chaves. Nessa parte, teremos todo o código que será executado quando uma função for chamada.
- Exemplo:
~~~
function traceParameter(aParam:String)
	{
	Trace(aParam);
	}
traceParameter(“Hello”);
~~~
			
#### Expressões de função

A segunda forma de declarar uma função é usar uma instrução de atribuição com uma expressão de função, que às vezes também é chamada de literal de função ou função anônima. Este método é mais detalhado e amplamente usado nas versões anteriores do ActionScript. Devem ser feitos os seguintes passos:<br>
	1) Utilizar a palavra-chave “var”;<br>
	2) Colocar o nome da função;<br>
	3) Adicionar o operador dois-pontos (:);<br>
	4) Classe “Function” para indicar os tipos de dados;<br>
	5) Operador de atribuição (=);<br>
	6) A palavra-chave “function”;<br>
	7) Definir os parâmetros em uma lista delimitada por vírgulas e parênteses;<br>
	8)Fazer o corpo da função, que deve ficar entre chaves. Nessa parte, teremos todo o código que será executado quando uma função for chamada.<br>
- Exemplo:
~~~
var traceParameter:Function = function(aParam:Sring)
	{
		Trace(aParam);
	}
traceParameter(“hello”);
~~~
Observe que um nome de função não é especificado da mesma forma que em uma instrução de função. Outra diferença importante as duas é que uma expressão de função não é suficiente como uma instrução de função.No exemplo seguinte, temos uma função de expressão atribuída a uma matriz:
~~~
var traceArray:Array = new Array();
traceArray[0] = function (aParam: string)
{
	Trace(aParam);
};
traceArray[0](“hello”);
~~~
#### Escolha entre instruções e expressões

Sempre utilize uma instrução de função, pois elas são menos detalhadas e fornecem uma experiência mais consistente, são mais fáceis de ler e tornam o código mais conciso, além de serem menos confusas do que as expressões de função, que requerem o uso das palavras-chave “var” e “function”. Porém, caso alguma circunstância específica exija o uso de uma expressão, utilize-a.<br>

As instruções de função fornecem uma experiência mais consistente entre os dois modos de compilação, já que é possível usar a sintaxe de pontos nos modos estrito e padrão para chamar um método declarado usando uma instrução de função. Isso não é necessariamente verdadeiro para métodos declarados com uma expressão de função. Por exemplo, o código a seguir define uma classe chamada Example com dois métodos: methodExpression(), que é declarado com uma expressão de função, e methodStatement(), que é declarado com uma instrução de função. No modo estrito, não é possível usar a sintaxe de pontos para chamar o método methodExpression().

~~~ 
Class Example
{
	var methodExpression = function() {}
	function methodStatement() {}
}

var myEx:Exemple = new Example();
myEx.methodExpression();
myEx.methodStatement();
~~~

As expressões de função são consideradas mais adequadas à programação que se concentra no comportamento em tempo de execução ou dinâmico. Se você preferir usar o modo estrito, mas também precisa chamar um método declarado com uma expressão de função, você pode usar uma das duas técnicas. Primeiro, você pode chamar o método usando colchetes ( [] ) Em vez do ponto ( . ) Operador. A chamada de método que se segue êxito no modo estrito e modo padrão:
~~~
MyExample ["methodLiteral"] ();
~~~
#### Retornando valores de funções

Para retornar um valor, é necessário utilizar "Return". Em seguida, coloque a expressão ou valor que deseja retornar.<br>

- Exemplo:
~~~
function doubleNum(baseNum:int):int 
{
    return (baseNum * 2);
}
~~~
#### Funções Aninhadas

Útil para declarar uma ou mais funções dentro de outra. Está disponível apenas dentro da função pai, a menos que uma referência a ela seja transmitida ao código externo.
~~~
function getNameAndVersion():String
{
    function getVersion():String
    { 
        return "10";
    }
    function getProductName():String
    {
        return "Flash Player";
    }
    return (getProductName() + " " + getVersion());
}
trace(getNameAndVersion());
~~~

### Referências
https://pt.wikipedia.org/wiki/ActionScript

http://www.adobe.com/devnet/actionscript/learning.html

http://help.adobe.com/pt_BR/ActionScript/3.0_ProgrammingAS3/WS5b3ccc516d4fbf351e63e3d118a9b90204-8000.html

http://help.adobe.com/pt_BR/ActionScript/3.0_ProgrammingAS3/flash_as3_programming.pdf

http://www.adobe.com/devnet/actionscript
