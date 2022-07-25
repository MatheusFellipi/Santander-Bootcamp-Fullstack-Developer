# Santander Bootcamp Fullstack Developer

Estudos realizando no Santander Bootcamp Fullstack Developer

<h1>Angular</h1>

<h3>Data Binding</h3>

O Angula trabalha com commponente modular.
Fortalece o html

- Interpolação: {{ valor }} associa informação do componente para o template (HTML)

- Property Binding: [propriedade]="valor" associa informação do componente para o template (HTML)

- Event Binding: (evento)="handler" associa informação do template (HTML) para o componente

- Two-Way Data Binding: [(ngModel)]="propriedade" associa informação entre ambos, ou seja, mantém ambos atualizados (componente e
  template (HTML).

<h3>Diretivas</h3>

As diretivas fornecem meios para que possamos manipular o DOM ou estender as funcionalidades do elemento.

- Diretivas de atributos: Alteram a aparência ou o comportamento de um elemento, componente ou outra diretiva, como por exemplo,
  `NgClass` e `NgStyle`.

- Diretivas estruturais: Modificam o layout adicionando ou removendo elementos do DOM, como por exemplo, `NgIf` e `NgFor`.

As diretivas são marcadores em um elemento DOM (como um atributo) que informam ao Angular para anexar um comportamento especificado a um elemento existente.
Existem muitas diretivas prontas que podemos usar e também podemos criar nossas próprias diretivas.

- `ngIf`: Esta é uma diretiva que você adiciona a um elemento na marcação, geralmente
  para um elemento de contâiner como um div.

- `ngFor`: Esta é uma diretiva para processar cada item de um objeto iterável, gerando uma
  marcação para cada um. Ela é conhecida como uma diretiva estrutural porque pode
  alterar o layout do DOM adicionando e removendo elementos DOM de visualização.

Input Property - @Input() Você irá utilizá-lo quando quiser receber dados de um componente pai.

Output Property - @Output() Você irá utilizá-lo quando quiser enviar dados de um componente filho para um
componente pai.

- [Código do estudos](https://github.com/MatheusFellipi/course-maneger)

<hr/>

<h3> SPA </h3>

Pode carregar os componentes sem a necessidade de carregar toda a pagina novamente.

- [Código do estudos](https://github.com/MatheusFellipi/course-maneger)

<h3> O que e componente? </h3>

A arquitetura de componentes baseia-se na construção de componentes independentes, substituíveis e modulares que auxiliem no gerencianciamento da complexidade e encorajem a reutilização.

- Seus benefícios incluem:

  - Escalabilidade

  - Manutenção

  - Performance

<h3> Serviços </h3>

Um serviço Angular reutilizável é projetado para encapsular a lógica de negócios e os dados com diferentes componentes do Angular. É basicamente uma classe que tem um propósito bem definido para fazer algo. Você pode criar uma classe de serviço para dados ou lógica que não está associada a nenhuma visualização específica para compartilhar entre os
componentes.

Se você escrever toda a lógica de negócios em componentes, terá os seguintes problemas:

- Você não poderá reutilizar essa lógica em nenhum outro lugar e terá que recodificar toda a lógica no componente de destino.

- A manutenção de seus componentes será difícil, pois você terá que manter duas cópias do mesmo código.

- Responsáveis por organizar e compartilhar lógica de negócios

- Reutilizáveis entre diferentes componentes de um aplicação

- Mandatorios para uma arquitetura modular e reutilizável

<h3> Ciclo de vida do Componente </h3>
Todo componente possui seu ciclo de vida (normalmente chamado de lifecycle hooks), que começa assim que Angular o instancializa na aplicação e através deles é possível executar diferentes lógicas nos vários
estágios de um componente.

<h3> Injeção de dependência</h3>

A injeção de dependência é usada para fornecer aos
componentes os serviços que eles podem usar. Para definir uma classe como um serviço no Angular, o decorator `@Injectable()` é usado.

Ele fornece os metadados que permitem ao Angular injetá-los em um componente como uma dependência.

Da mesma forma, o decorator `@Injectable()` é usado para indicar que um componente ou outra classe (como outro serviço, um pipe ou um NgModule) possui uma dependência.

Todo serviço é uma dependência que precisa ser instanciada dentro do componente para ser utilizada pelo mesmo. No angular, o componente pede para aplicação quais dependências ele precisa e então as injeta dentro de si.

<h3>Constructor vs ngOnInit</h3>

- Constructor

  - Deve ser utilizado apenas para inicializar serviços injetados via DI (injeção de dependência)

- ngOnInit
  - Deve ser utilizado para todo tipo de lógica que o componente precisar executar após ter sido criado.

<h3>@Input()</h3>
* Pai -→ Filho:
  
- Principal maneira de compartilhar dados do pai para filho:

<h3> @Output() e EventEmitter </h3>
* Filho → Pai:

- Principal maneira de compartilhar dados do filho para o pai:

<h3> Componentes apresentacionais </h3>
- Parecido com funções puras
- Se preocupam apenas com a interface do usuário
- Não ficam responsáveis por recuperar dados ou lidar com lógica de negócio
- Não causam efeitos colaterais na aplicação
- Recebem dados via @Input e emite eventos via @Output
<h3> Componentes inteligentes </h3>
- Parecido com funções impuras
- Contém toda a lógica de negócio
- São internamente compostos por componentes
apresentacionais
- Ficam responsáveis por repassar os dados para os
componentes apresentacionais apresentaram ao usuário final

<h3>Design Modular</h3>

- Dividisão da aplicação web em módulos de recursos que representam diferentes funcionalidades de negócios.

- Core Module: define serviços singleton, componentes de instância única, configuração e exportação de quaisquer módulos de terceiros necessários no módulo principal (App Module).

- Shared Module: contém componentes/pipes/diretivas comuns e também exporta módulos do Angular usados com frequência (CommonsModule)

- Feature Module: organiza um conjunto de recursos da aplicação num módulo de funcionalidade.
- Library: possui código que pode ser reutilizável entre diferentes aplicações.

- Angular Element: recurso do angular para criar web components, padrão da web para definir novos elementos HTML de uma maneira independente de estrutura e agnóstica de frameworks.

<h3> SMACSS </h3>

SMACSS é uma arquitetura modular e escalável para CSS, dividida

em 5 camadas. Sendo elas:

- Base: estilização de seletores e pseudo-classes, além de resets

- Layout: principais componentes como cabeçalho, rodapé, entre outros.

- Module: componentes reutilizáveis como botões e ícones.

- State: todo elemento que será modificado ou terá alguma alteração no seu estado inicial.

- Theme: temas específicos para uma mesma aplicação.

<h3> BEM CSS </h3>

A sigla BEM significa block, element, modifier (bloco, elemento e modificador) , sendo uma metodologia que segue esses conceitos para definir uma nomenclatura de nomes para classes CSS.

<h3> OOCSS </h3>

O OOCSS (CSS orientado à objeto) é uma metodologia que identifica um
padrão visual que pode se repetir no projeto e o agrupa em classes,
tornando-os reutilizáveis.

<hr/>

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
- Java ME (java Platform, Micro edition) cuida para dispositivo mobile e embarcados .

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

- Tipos

  - Instancia: Objeto.
  - Classe: Classe.
  - Local: dentro do métodos.
  - Parâmetros: na assinatura do método.

- Padrão de definição
<?visibilidade?><?modificador?>tipo nome <?=ValorInicial?>;

V: public protected e private.
M: static e final.
T: tipo de dado.  
N: nome que e fornecido a variável.
VI: um valor inicial, caso se deseje.

- Sempre tenho boa pratica na criação das variáveis.

<h4>tipos de dados</h4>

- Sao os valores e consequentemente operações que as variáveis podem assumir e sofrer respectivamente.

- Tipificação

  - Estática(forte) vs Dinâmica(fraco)

    - Estática voce e Obrigado a definir o tipo dela na criação a dinâmica ela permite alterar o tipo durante a execução.

  - Primitivo vs Composto
    - os dados primitivo sao valores numéricos, texto..., sao dados básico que todas as linguagens, os tipos composto sao heterogenia, pode der vários tipo de dados na estrutura.

- Operadores Aritméticos

* Sao símbolos especiais quais sao capazes de realizar acoes especificas em um, dos ou mias operandos e, em seguida, retorna um resultados.

* Tipos
* Pos-fixado: exp++ ou exp--
* Prefixado: ++exp ou --exp
* Aritmético: +, -, \*, /, %
* Atribuição: =, +=, -=, \*=, /= e %=

- as prioridade das execução sao:
  - Pos-fixado: exp++ ou exp--
  - Prefixado: ++exp ou --exp
  - Múltiplo: \*, /, %
  - Aditivo: +, -,
  - Atribuição: =, +=, -=, \*=, /= e %=

<h3>Conversões(Casting)</h3>

- E a transformação de um determinada variável de tipo menos específicos para um tipo mais especifico

- Tipos
  - IpCast(Implícito)
  - Downcast(Explicito)

<h3>Métodos</h3>

- E um porcão de código (sub rotina) que e disponibilizada por uma classes. Este e executado quando e feita um requisição a ele. sao respostáveis por definir e realizar um determinado comportamento

- Padrão de definição
<?visibilidade?><?tipo?><?modificador?>retorno nome (<?parâmetro?>)<?exceções?>corpo;

V: public protected e private.
T: concreto ou abstrato.
M: static e final.
R: tipo de dado ou void.  
N: nome que e fornecido ao métodos.
P: parâmetro que pode receber.
E: Exceções que pode lançar.
C: código que possui ou vazio

- Particularidade

  - assinatura: e a forma de identificar unicamente o metodo
    - ass = nome + parâmetros

- passagem de parâmetros

  - Por valor (cópia)
  - por referência(endereço)

- Atividade

  -Cria uma aplicação que resolva as seguintes situações:

  - Calcule as 4 operações básicas: soma, subtração, multiplicação e divisão. Sempre 2 valores devem ser passados.

  - A partir da hora do dia, informe a mensagem adequada: Bom dia, Boa tarde e Boa noite.

  - Calcule o valor final de um empréstimo, a partir
    do valor solicitado. Taxas e parcelas influenciam.
    Defina arbitrariamente as faixas que influenciam
    nos valores.

    - Resolução:
      [Exercícios realizado](https://github.com/MatheusFellipi/DIO_Atividade_Java_Curso_metodo)

     <h3>Sobre carga</h3>

  - E a capacidade de definir métodos para diferente contextos, mais preservando seu nome.

  - O nome se mandem e muda apenas os parâmetros

  - Cria uma aplicação que calcula a área dos 3 quadriláteros notáveis: quadrado, retângulo e trapézio.
    - Obs: Use sobrecarga.

  * Resolução:
    [Exercícios realizado](https://github.com/MatheusFellipi/DIO_Atividade_Java_Curso_metodo)

<h3> Retorno </h3>

- Retorno - É uma instrução de interrupção
- Simbologia: return
  \*O continue e o break também são instruções de interrupção, mas estão mais atrelados a laços de repetição e o retorno está atrelado a métodos.

- O método executa seu retorno quando:
  - Completa todas suas instruções internas
  - Chega a uma declaração explícita de retorno
  - Lança uma exceção

\*O tipo de retorno do método é definido na sua criação e pode ser um tipo primitivo ou objeto;

- O tipo de dado do return deve ser compatível com o do método;
- Se o método for sem retorno(void), pode ou não ter um "return" para encerrar sua execução.

Recrie a aplicação que calcula a área dos 3 quadriláteros notáveis. Agora faça os métodos retornarem valores.

- Resolução:
  [Exercícios realizado](https://github.com/MatheusFellipi/DIO_Atividade_Java_Curso_metodo)

<h3>Operadores relacionais</h3>

- sao símbolos especiais quais sao capazes de realizar comparações entre determinados operados , em seguida, retorna um resultado.

- Similaridade

  - Igualdade: determina se o operado e igual au outro.
  - Diferençá: determina se o operado e nao igual au outro.

- Tamanho
  - Maior: determina se o operado e maior au outro.
  - Maior igual: determina se o operado e maior ou igual ao outro.
  - Menor: determina se o operado e menor au outro
  - Menor igual: determina se o operado e menor ou igual ao outro.

<h3>Operadores lógicos</h3>
* Sao simbolo especiais quais sao capazes de realizar comparações logicas entre operandos lógicos ou expressões e, em seguida, retorna um resultado

<h3>Controle de fluxo</h3>
* sao estrutura que tem a capacidade de direcionar o fluxo de execução do código.

<h3>Blocos</h3>
* e um grupo de 0 ouo mias código quais trabalham em conjunto para executar uma operação

<h3>Estrutura de Repetição</h3>
* uma estrutura de repetição permita que um sequencia de comando seja executada repetidamente, caso determinadas coedições seja satisfeita

- Repetição com teste no inicio (while)
- Repetição com teste final (do-while)
- Repetição contada (for)
  - Break e utilizado para terminar de forma abrupta um repetição
  - Continue e for executado ele volta para testar novamente ou nao.

[Atividade realizada](https://github.com/MatheusFellipi/DIO_Atividade_Loops)

<h3>Collections</h3>

- Collection é um objeto que agrupa múltiplos elementos
  (variáveis primitivas ou objetos) dentro de uma única unidade.

- Serve para armazenar e processar conjuntos de dados de
  forma eficiente.

- Interfaces: É um contrato que quando assumido por uma
  classe deve ser implementado.

- Implementações ou Classes: são as materializações, a
  codificação das interfaces.

- Algoritmos: É uma sequência lógica, finita e definida de
  instruções que devem ser seguidas para resolver um problema.

<h4>java.util.List</h4>
* Elementos duplicados e garante ordem de inserção

- ArrayList deve ser usado onde mais operações de pesquisa são necessárias, e LinkedList deve ser usado onde mais operações de inserção e exclusão são necessárias.

[Atividade de lista](https://github.com/MatheusFellipi/DIO_estudos_List)

<h3>Tratamento de erro</h3>

- identificar possíveis exceções de um aplicação Java e interpretar eventuais pilhas de exceção
- Exceção é um evento que interrompe o fluxo normal do processamento de uma classe.
- O uso correto de exceções torna o programa mais robusto e confiável.
  Com o tratamento de exceções, um programa pode continuar executando depois de lidar com um problema.
- Importante: Incorpore sua estratégia de tratamento de exceções no sistema desde o princípio do processo do projeto.
- Pode ser difícil incluir um tratamento de exceções eficiente depois que um sistema foi implementado.
- Error: Usado pela JVM que serve para indicar se existe algum problema de recurso do programa, tornando a execução impossível de continuar.
- Unchecked (Runtime): Exceptions que PODEM ser evitados se forem tratados e analisados pelo desenvolvedor.
- Checked Exception: Exceptions que DEVEM ser evitados e tratados pelo desenvolvedor para o programa funcionar.
- Para trabalhos com exceções usa o try catch finally.

[Os exemplo de Tratamento de erro ](https://github.com/cami-la/exceptions-java)

<h3>Debugging java</h3>

Erros de programação são denominados bugs e o processo de encontrar e corrigir bugs é chamado de depuração ou debugging.

[Código usando para teste de Debugging](https://github.com/cami-la/debugging-java)

<h1> String Boot <h1>

Para um arquivo de confirugacao e necessário definir ele como arquivo de configuracao
`@Configuration` e ``@configurationProperties("spring.datasouce")` mapea as configuracao do ambiente.

Para configuracaoo banco de dados com um ambiente de desenvolvimento e protucao
usar o `@profile("Ambiente")` para essa configuracao.
