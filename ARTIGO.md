# RUBY
<br />

---
## História
---

&nbsp;&nbsp;&nbsp; A linguagem Ruby nasceu em 23 de fevereiro de 1993 por Yukihiro Matsumoto ("Matz") que pretendia criar uma nova linguagem que balanceava programação funcional com a programação imperativa. Matsumoto afirmou: "Eu queria uma linguagem de script que fosse mais poderosa do que Perl, e mais orientada a objetos do que Python. É por isso que eu decidi desenvolver minha própria linguagem.". O nome Ruby foi decidido durante uma sessão de bate-papo online entre Matsumoto e Keiju Ishitsuka em 24 de fevereiro de 1993, antes que qualquer linha de código tivesse sido escrita para a linguagem. Inicialmente foram propostos dois nomes: "Coral" e "Ruby", sendo esse último nome proposto escolhido mais tarde por Matz em um e-mail para Ishitsuka. Matsumoto explicou mais tarde que o motivo de ter escolhido o nome "Ruby" foi porque essa era a pedra zodiacal de um de seus colegas.

&nbsp;&nbsp;&nbsp; Matz pensou o Ruby como uma linguagem fácil de usar e genuinamente orientada a objetos, ao contrário de Python que segundo sua opinião não era naturalmente orientada a objetos já que suas funcionalidades para esse fim pareciam ser "add-on". Ele usou partes de suas linguagens favoritas para criá-la - Smalltalk, Eiffel, Ada, Lisp e Perl - esta última teve suas funcionalidades usadas como base para a criação das bibliotecas de classe do Ruby.

&nbsp;&nbsp;&nbsp; Ruby se tornou uma linguagem pública em dezembro de 1995, com o release da versão 0.95 no Japão. Em 1998, visando expandir o uso da linguagem globalmente, foi criada a primeira lista de discussões, o Ruby-Talk. Em 1999 Matz escreveu o primeiro livro sobre programação em Ruby e em 2001 foi lançado o primeiro livro em inglês, tornando a linguagem acessível a um público maior. A "decolagem" do Ruby veio em 2005 com a criação do Ruby on Rails, um framework que faz o desenvolvimento, implantação e manutenção de uma aplicação web mais fácil. Desde então a aceitação da linguagem não parou de crescer resultando na formação de grupos de usuários em todas as principais cidades do mundo e com as conferências sobre Ruby com lotação esgotada.
<br />
<br />
<br />
 
 
---
## Características
---

&nbsp;&nbsp;&nbsp;* Linguagem interpretada.<br />
&nbsp;&nbsp;&nbsp;* Multiparadigma.<br />
&nbsp;&nbsp;&nbsp;* Tipagem forte e dinâmica.<br />
&nbsp;&nbsp;&nbsp;* Gerenciamento automático de memória.<br />
&nbsp;&nbsp;&nbsp;* Multiplataforma.<br />
&nbsp;&nbsp;&nbsp;* Open-source.
<br />
<br />
<br />


---
## Principais Usos
---

&nbsp;&nbsp;&nbsp; Por ser uma linguagem considerada genérica seu uso é bem diversificado, mas o Ruby tem sido mais utilizado como ferramenta de desenvolvimento WEB, graças em grande parte ao framework Ruby on Rails ou ROR. Por ser Open source e ter uma comunidade ativa, muitas startups optam por desenvolver suas aplicações em Ruby / RoR, pois conseguem adaptar e alterar o seu código de forma ágil. Por seu dinamismo e com códigos simples e constantemente descritos como elegantes tornando seu entendimento mais fácil que outras linguagens, ela vem atraíndo cada vez mais atenção. Plataformas populares foram construídas sobre seus códigos, como por exemplo twitter, airbnb, shopify, github, hulu e slideshare. Algumas outras aplicações do Ruby são:
<br />

&nbsp;&nbsp;&nbsp;**Criação de simulações** - Um grupo de pesquisa na Motorola usa Ruby para fazer scripts para um simulador, tanto para gerar cenários como para processar esses mesmos dados depois. <br />

&nbsp;&nbsp;&nbsp;**Modelagem 3d** - O Google SketchUp é uma aplicação de modelagem 3D que utiliza o Ruby para sua macro-API de scripting. <br />

&nbsp;&nbsp;&nbsp;**Gestão de Negócios** - Toronto Rehab usa um programa baseado no RubyWebDialogs para gerir e acompanhar o suporte via telefone e pessoal das equipes de help desk de TI e operações de TI. <br />

&nbsp;&nbsp;&nbsp;**Robótica** - No projeto MORPHA, Ruby foi usado para implementar a parte do controle reativo do robô de serviços da Siemens.<br />

&nbsp;&nbsp;&nbsp;**Redes** - O Open Domain Server usa Ruby de forma a permitir que as pessoas usem clientes de DNS Dinâmicos para a atualização em tempo real das configurações de IP para que possam ser mapeadas em domínios estáticos.<br />

&nbsp;&nbsp;&nbsp;**Telefonia** - Ruby está sendo utilizado na Lucent num produto de telefonia 3G wireless.<br />

&nbsp;&nbsp;&nbsp; **Administração de Sistemas** - Ruby foi usado para escrever o componente de coleta de dados do sistema de Capacidade unix e Planejamento da Level 3 Communications, que recolhe estatísticas de performance de cerca de 1700 servidores Unix (Solaris e Linux) espalhados pelo mundo.<br />

&nbsp;&nbsp;&nbsp;**Segurança** - O Metasploit Framework, um projeto open source da comunidade gerenciado pela Rapid7, é uma plataforma gratuita de teste de penetração que permite que profissionais de TI avaliem a segurança de suas redes e aplicações. O projeto Metasploit consiste de mais de 700.000 linhas de código e foi baixado mais de um milhão de vezes em 2010. As versões comerciais desenvolvidas pela Rapid7 também são baseadas em Ruby.<br />
<br />
<br />


---
## Expressividade
---

&nbsp;&nbsp;&nbsp; Uma de suas principais características é a expressividade que possui. O desenvolvimento da linguagem Ruby teve como objetivo desde o início que fosse uma linguagem muito simples de ler e ser entendida, para facilitar o desenvolvimento e manutenção de sistemas escritos com ela. Exemplos de expressividade:

**Métodos que retornam true ou false terminam com uma interrogação em seu nome**

|&nbsp;&nbsp;animais = ["cachorro","gato","cavalo"]&nbsp;&nbsp;&nbsp;<br />
|&nbsp;&nbsp;print animais.**include?** "gato"&nbsp;&nbsp;&nbsp; *#Verifica se existe gato na array e imprime TRUE na tela*<br />
<br />

**Métodos que alteram o objeto são terminados com ponto de exclamação**

|&nbsp;&nbsp;animais = ["cachorro","gato","cavalo"]<br />
|&nbsp;&nbsp;animais.**slice!(1)**&nbsp;&nbsp;&nbsp; *#Retira o valor no índice 1 do array*<br />
|&nbsp;&nbsp;print animais.include? "gato"&nbsp;&nbsp;&nbsp; *#Imprime FALSE na tela*<br />
<br />

**Métodos "attribute accessors" para manipulação de atributos de um objeto**

|&nbsp;&nbsp;class Bichos<br />
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**attr_accessor :animais**&nbsp;&nbsp;&nbsp; *#Equivalente a criar o atributo animais e os métodos animais e animais=*<br />
|&nbsp;&nbsp;end<br />
|&nbsp;&nbsp;<br />
|&nbsp;&nbsp;exemplo = Bichos.new()&nbsp;&nbsp;&nbsp;<br />
|&nbsp;&nbsp;exemplo.**animais =** ["cachorro","gato","cavalo"]&nbsp;&nbsp;&nbsp;<br />
|&nbsp;&nbsp;print exemplo.**animais**&nbsp;&nbsp;&nbsp;<br />
<br />

**As variáveis, por serem instâncias, possuem métodos que facilitam desenvolvimento em Ruby**

|&nbsp;&nbsp;def pares(limite)&nbsp;&nbsp;&nbsp;<br />
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.**upto(limite)** {&nbsp;&nbsp;&nbsp;*#1 é uma instância da classe Fixnum e chama o método "upto" equivalente ao FOR*<br />
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|i| puts i if i % 2 == 0<br />
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br />
|&nbsp;&nbsp;end<br />
|<br />
<br />
O trecho em Java seria:
<br />

|&nbsp;&nbsp;public void pares(int limite){&nbsp;&nbsp;&nbsp;<br />
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for(int i = 1; i<= limite; i++){<br />
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if(i % 2) System.out.println(i);<br />
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br />
|&nbsp;&nbsp;}<br />






<br />
<br />

---
## Bibliografia
---
Wikipedia - Ruby(linguagem de programação): https://pt.wikipedia.org/wiki/Ruby_(linguagem_de_programa%C3%A7%C3%A3o)<br />

Sitepoint - The History of Ruby: https://www.sitepoint.com/history-ruby/<br />

Ruby - Sobre o Ruby: https://www.ruby-lang.org/pt/about/<br />

DEVMEDIA - Ruby on Rails Tutorial: https://www.devmedia.com.br/ruby-on-rails-tutorial/31285<br />

DEVMEDIA - Conhecendo a Linguagem Ruby: https://www.devmedia.com.br/conhecendo-a-linguagem-ruby/8226<br />

EU SOU DEV - Dúvida cruel: Ruby ou PHP?: https://eusoudev.com.br/ruby-ou-php/<br />

Caelum - A linguagem Ruby: https://www.caelum.com.br/apostila-ruby-on-rails/a-linguagem-ruby/#2-1-a-historia-do-ruby-e-suas-caracteristicas<br />

Arthur de Moura Del Esposte - Orientação a Objetos com Ruby: https://www.ime.usp.br/~esposte/documents/aula-ruby/aula01/Aula01.pdf<br />

Carlos Henrique Costa Junior, Daniel de Andrade, Darlan Pedro de Campos e Guilherme Silvestre Gomes - Ruby: https://www.inf.ufsc.br/~frank.siqueira/INE5612/Seminario2010.1/Ruby.pdf






