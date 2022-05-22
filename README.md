# <P align="center">**CURSO <font color="red">AGULAR</font>**</P>

# <p align="center">Nesse curso aprendemos os recursos fundamentais do framework e depois criaremos do zero um projeto fullstack.<p>

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169174026-26ebb9ac-1fb4-4949-913a-11551fafa700.png"/></P>

## 📝 O que é Angular?

- Um framework com base na linguagem JavaScript;
- Utilizado para criação de SPAs;
- Possui arquitetura baseada em componentes;
- Muito utilizando em aplicações de grande porte;
- Angular 2+ é uma visão diferente so AngularJS (clássico);

## 📝 Tecnologias

- HTML e CSS
- TypeScript
- JavaScript
- Node
- npm

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/167973345-8988dcdc-0b90-49c6-a584-3b6d2045df9a.png"/></P>

## 📝 Interpolação de dados / Dados no template

<p align="center">Vamos colocar dados da classe do componente no nosso template de Angular.
Este recurso é conhecido como interpolação, e é utilizado em todos os projetos que criamos com este framework
Ou seja, é um assunto muito importante, que você precisa dominar</p>

- A interpolação de dados é um recurso que vai nos ensinar a trabalhar com os componentes do Angular;
- Vamos criar nossas variáveis no arquivo .ts, dentro da classe;
- Ou seja, estas variáveis são propriedades da classe;
- E então teremos acesso a estes dados no arquivo .html, o template;
- A impressão é feita através de: {{dado}}

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169178385-e1ef24ff-280b-43d6-b066-cc71cfb4e8ec.png"/></P>

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169178187-5dcdc55e-d3f8-4ffd-ac64-e3e21915f2a2.png"/></P>

## 📝 CSS no Angular
<p align="center">Nesta você vai aprender as maneiras de adicionar #CSS no #Angular
Isso será reaproveitado nas aulas dos nosso projetos, ondem todos precisam de um pouco de estilos.</p>

- Os estilos em aplicações de Angular podem ser feitos de duas maneiras;
- Global: utilizando o arquivo styles.css, que fica em src;
- Scoped: estilos a nível de componente, criamos quando damos um generate;

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169181980-49575082-745f-4639-9ea0-cf59a487983e.png"/></P>

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169182014-d5298bfd-8cb8-4af6-b02e-971007bc0cd3.png"/></P>

## 📝 Compartilhando dados
<p align="center"> Compartilhamento de dados do componente pai para o componente filho em #Angular
Este recurso em outros frameworks front-end é chamado de props
E nos possibilita trabalhar com componentes dinâmicos, baseado em dados diferentes passados.</p>

No terminal com o comando abaixo criamos novo component com nome parent-data.

-- ng generate component components/parent-data

- Em Angular podemos compartilhar dados do componente pai com o componente filho;
- Para isso, vamos disponibilizar na chamada do componente o nome do dado que será recebido com a seguinte sintaxe: [dado];
- E no código .ts do componente filho vamos utilizar o decorator @input, que tem papel entregar o dado para o template;

## 📝 Diretivas do Angular
<p align="center"> Recurso chamado diretivas, que é super importante para o #Angular Com podemos criar funcionalidades complexas no nosso app.</p>

- Em Angular temos um recurso chamado diretivas;
- Que podem realizar diversas funções no sistema, como aplicar estilos a em elemento;
- Elas começam sempre com ng, o nome fica como: ngAngularCoisa;

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169426021-4bfb2f3a-5db0-4c2f-b031-6926205fc3db.png"/></P>

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169426210-5ca030a8-a7b5-49c1-a71f-4f3f250f87ce.png"/></P>

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169426276-3ee1899d-bd7a-436f-a6d1-61a0c3cca650.png"/></P>

## 📝 Renderização condicional
<p align="center"> Criando uma renderização condiconal em Angular
Ou seja, imprimir algo no template baseado em uma condicional if e else
Isso nos permite mais flexibilidade ainda com o framework.</p>

- É possível exibir determinado conteúdo por meio de uma condicional;
- Utilizamos a diretiva nglf para isso;
- Os valores podem ser dinâmicos (propriedades), mas podemos realizar outros tipos de comparação;
- Há a possibilidade também de imprimir um cenário para avalização de falso, com o else;

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169435349-f3d5f518-9828-4e5b-acc6-6bd0880d18c7.png"/></P>

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169435522-a2f86757-5a50-44ff-b541-57e0b14ebb8b.png"/></P>

## 📝 Eventos no Angular
<p align="center"> Os eventos em frameworks de front-end são recursos essenciais
Um dos mais utilizados é o de click, quando o usuário clica em algum elemento e dispara uma função.</p>

- Podemos ativar eventos nos componentes para disparar algum método;
- Um evento clássico que utilizamos muito é o click;
- A sintaxe é: (click)="algumaFuncao()"
- Os métodos ficam na classe;
- Futuramente utilizaremos este recurso para acessar uma API;

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169658114-4e850f03-1aef-4624-ad76-907a17532c74.png"/></P>

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169658149-4660402c-d8b6-4398-8a32-e8e78182eb7c.png"/></P>

## 📝 Emitindo eventos
<p align="center"> Esta técnica consiste em conseguir ativar um evento em um componente filho, e replicar isso para o componente pai
Desta maneira conseguimos executar uma função que é controlada por outro componente.</p>

- Podemos comunicar eventos de um componente filho para o pai;
- Para isso vamos precisar o @Output. que vai fazer a saída do evento do componente filho;
- Na tag invocação do componente no template, escolhemos um método para executar quando o evento for emitido;
- Exemplo: (emit)="onEmit"

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169658114-4e850f03-1aef-4624-ad76-907a17532c74.png"/></P>

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169658149-4660402c-d8b6-4398-8a32-e8e78182eb7c.png"/></P>

## 📝 Renderização de listas
<p align="center"> O recurso consiste em ter um array, geralmente de objetos, onde iteramos por cada um dos itens
E imprimimos suas informações no template, exemplo: Uma lista de produtos da home de um e-commerce.</p>

- Outro recurso importante é o loop em listas;
- Para isso vamos precisar de uma propriedade com os itens da lista;
- E no template do componente vamos utilizar o *ngFor;
- A sintaxe é: *ngFor="let item of items";
- Desta maneira podemos renderizar template baseado em dados;

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169676473-720d29dc-e2cc-4cd3-bb92-733c4a75924e.png"/></P>

 <p align="center">
<img src="https://user-images.githubusercontent.com/79487813/169676488-23dd22a6-553c-428b-b6af-50c994dd17fa.png"/></P>


