# Santander Bootcamp Fullstack Developer
 Estudos realizando no Santander Bootcamp Fullstack Developer



<h1>Java</h1>

- E um linguagem de orientação a objeto.
- um linguagem interpretada .

<h3>Fase de execução do java</h3>
<div style={{
  display: 'flex',
  justifyContent: 'center',
  alignItems: 'center',
}}>
![010102_imagem031](https://user-images.githubusercontent.com/47674343/172265799-a9399ff7-b387-4c1c-a943-cd7fa7a709b4.png)
</div>

<p>
java e um linguagem compilada para bytecode e interpretada pelo um maquina virtual JVM.
</p>

<hr/>

<h3>Plataforma X linguagem</h3>
<p>
  a linguagem java nao e a única da sua plataforma mais e a mais convencional .
</p>

- Groovy (segunda linguagem desenvolvida).
- JRuby.

<p>
  A vantagem  da plataforma e que nao fica preso a único sistema operacional ou hardware, pois roda um maquina virtual.
</p>

- escreva um vez e executa em qualquer lugar.

- Java SE (java Platform, standard edition) base da plataforma.
- Java EE (java Platform, Enterprise edition) cuida do desenvolvimento web.
- Java ME (java Platform, Micro edition)  cuida para dispositivo mobile e embarcados .

<h3>JDK X JRE</h3>

- JDK (java development kit ) e o kit de desenvolvimento java responsável por compila o código-fonte (.java) em bytecode (.class).
- JVM (Java virtual machine) e a maquina virtual do java responsável por executar o bytecode.
- JRE (Java Runtime Environment) Ambiente de execução do java que fornece as biblioteca padro do java para o JDK compilando o código para a JVM.

<h3>Versões java</h3>
- OpenJDK código aberto.
- JDK Oracle Paga.


<h3>O que e IDE?</h3>
-IDE (Ambiente de desenvolvimento integrado).

<h3>Variável do java</h3>
- variável e um espaços na memoria do comportador, onde se pode guarda valors.

* Tipos
  - Instancia: Objeto.
  - Classe: Classe.
  - Local: dentro do métodos.
  - Parâmetros: na assinatura do método.


* Padrão de definição
<?visibilidade?><?MOdificador?>tipo nome <?=ValorInicial?>;

V: public protected e private.
M: static e final.
T: tipo de dado.  
N: nome que e fornecido a variável.
VI: um valor inicial, caso se deseje.

* Sempre tenho boa pratica na criação das variáveis.

<h4>tipos de dados</h4>

* Sao os valores e consequentemente operações que as variáveis podem assumir e sofrer respectivamente.

* Tipificação 
  - Estática(forte) vs Dinâmica(fraco)
    - Estática voce e Obrigado a definir o tipo dela na criação a dinâmica ela permite alterar o tipo durante a execução.

  - Primitivo vs Composto
    - os dados primitivo sao valores numéricos, texto..., sao dados básico que todas as linguagens, os tipos composto sao heterogenia, pode der vários tipo de dados na estrutura.

* Operadores Aritméticos
 - Sao símbolos especiais quais sao capazes de realizar acoes especificas em um, dos ou mias operandos e, em seguida, retorna um resultados.

 - Tipos
  - Pos-fixado: exp++ ou exp--
  - Prefixado: ++exp ou --exp 
  - Aritmético: +, -, *, /, %
  - Atribuição: =, +=, -=, *=, /= e %=

  * as prioridade das execução sao:
    - Pos-fixado: exp++ ou exp--
    - Prefixado: ++exp ou --exp 
    - Múltiplo: *, /, %
    - Aditivo: +, -, 
    - Atribuição: =, +=, -=, *=, /= e %=

<h3>Conversões(Casting)</h3>

```
 E a transformação de um determinada variável de tipo menos específicos para um tipo mais especifico
```
* Tipos 
  - IpCast(Implícito)
  - Downcast(Explicito)

<h3>Métodos</h3>


`E um porcão de código (sub rotina) que e disponibilizada por uma classes. Este e executado quando e feita um requisição a ele. sao respostáveis por definir e realizar um determinado comportamento
`
