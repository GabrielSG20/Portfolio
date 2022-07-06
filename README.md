<html>
<body>
  
 <h1 align="center"> Portfólio API's Banco de Dados</h1>
 
  <p align="center">
   <a href="#-api-1º-semestre"> 1º Semestre</a> •
    <a href="#-api-2º-semestre"> 2º Semestre</a></a> •
    <a href="#-api-3º-semestre"> 3º Semestre</a></a> •
   <a href="#-api-4º-semestre"> 4º Semestre</a> •
   <a href="#"> 5º Semestre</a></a> •
   <a href="#"> 6º Semestre</a></a>
  </p>
  
  ---
  
  <h2> Autor :necktie: </h2>
  <table align="center">
   <tr>
    <td align="center"><a href="https://www.linkedin.com/in/gabrielsoaresgoncalves/"><img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/GabrielSoares.jfif" width="200px;" alt=""/><br/><b>Gabriel Soares</b></a>
      <br/>
      Back-end Developer / Scrum Master
     </td>
   </tr>
  </table>

 ---
 
 <h2 align="center"> API 1º Semestre</h2>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> Aplicação Mobile voltada para facilitar o uso de smartphones para usuários da terceira idade. Após o aplicativo ser instalado pelo usuário em seu smartphone, ao clicar em seu ícone será aberta a tela inicial contendo um microfone como botão e um ícone de visualização de lista. Ao clicar no microfone, será gerado a tela de reconhecimento de voz da Google que irá captar o comando falado pelo usuário, acionando uma das funcionalidades. O ícone de visualização de lista, quando clicado, tem a função de mostrar as funcionalidades disponíveis para o usuário por meio de uma nova tela no aplicativo. Para mais informações sobre o projeto, acesse: <a href="https://github.com/Gil-cos/Projeto_Integrador_1-Sem2020">Assistente Virtual</a>.</p>
  <p align="justify" style="font-family:roboto;"> As funcionalidades de comando de voz desenvolvidas foram: 
  <ul>
    <li>Abrir câmera para tirar fotos.</li>
    <li>Realizar chamadas para o número de emergência.</li>
    <li>Configurar conectividade com redes Wi-Fi.</li>
    <li>Adicionar alarmes.</li>
    <li>Abrir o navegador para pesquisas na WEB.</li>
    <li>Adicionar novos contatos.</li>
    <li>Efetuar ligações.</li>
  </ul>
 </p>
  
  <h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
   
  <ul>
  <li><a href="https://www.java.com/pt_BR/">Java</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Linguagem de programação utilizada para o desenvolvimento Back-End do sistema, apresenta como principais características: Portabilidade, Robustez, Segurança, Orientação a Objetos, Dinâmica e Alto Desempenho. Foi um requisito técnico solicitado pelo cliente.</p></li>
  </ul></li>
   <li><a href="https://developer.android.com/studio">Android Studio</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Ambiente de desenvolvimento integrado para elaboração de aplicações Android nativas. Tendo o Java como linguagem back-end e XML para front-end.</p></li>
  </ul></li>
  <li><a href="https://trello.com/https://trello.com">Trello</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Foi utilizado como ferramenta do método Scrum para distribuição das atividades do grupo e priorização das demandas. Possibilitando realizar o planejamento das sprints, sendo capaz de registrar o progresso da equipe e do projeto, facilitando o desenvolvimento e acompanhamento da realização de tarefas. </p></li>
  </ul></li>

  </ul>
  
  <h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  
  <h3> Atribuições como Desenvolvedor Back-end</h3>
  <p align="justify" style="font-family:roboto;"> Como Desenvolvedor Back-End, as atribuições foram relacionadas com a elaboração da lógica do sistema planejado, tendo em vista as regras de negócio proporcionadas pela problemática. Criando os métodos que serão chamados pelo Front-End, obtendo uma solução completa com todas as funcionalidades necessárias. Como demonstrado no tópico de Tecnologias Adotadas, foi utilizado Java para o desenvolvimento Back-End, portanto os próximos parágrafos irão descrever a minha experiência em contribuir com a lógica do projeto.</p>
  
  <p align="justify" style="font-family:roboto;"> O primeiro passo foi a criação e configuração do ambiente que iríamos utilizar, fizemos criando um novo projeto na IDE Android Studio. Após isso, realizei a implementação do método catchSpeech(), que utiliza um objeto da classe Intent para capturar os comandos de voz falados pelo usuário. Esse objeto intent tem como função solicitar uma ação de outros componentes do Android, nesse caso está sendo requeriada a ação de reconhecimento de voz (ACTION_RECOGNIZE_SPEECH).</p>
   <details>
    <summary>Método catchSpeech</summary>
    <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/catchSpeech.png" width="800px;" alt=""/>
  </details>
  <p align="justify" style="font-family:roboto;"> Para finalizar o catchSpeech(), é chamado dentro de um try/catch (para capturar possíveis erros do software ou da fala do usuário) outro método nomeado startActivityForResult(). Responsável por verificar a resposta do intent e atribuí-la a uma variável (speech), chamando o método processMachineLearning().</p>
  <details>
    <summary>Método onActivityResult()</summary>
    <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/onActivityResult.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> O processMachineLearning() chamará os métodos que ativam as funcionalidades requeridas, de acordo com o comando falado.</p>
    <details>
    <summary>Método processMachineLearning()</summary>
    <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/processMachineLearning.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> Fui responsável pela criação de métodos relacionados com as funcionalidades de realizar chamadas para um número de emergência, realizar uma pesquisa na Web e indicar um filme ao usuário.</p>
  <p align="justify" style="font-family:roboto;"> A realização da chamada de emergência e pesquisa Web foram elaborados utilizando um objeto da Classe Intent, chamando ação necessária para cada um (ACTION_CALL e ACTION_WEB_SEARCH).</p>
    <details>
    <summary>Métodos callSOS() e searchGoogle()</summary>
    <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/metodosFuncionalidades.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> Já a recomendação do filme foi realizada por meio da consulta em uma API Https. Foi criada uma classe de serviço que estabele uma conexão com a URL a ser consumida e captura sua resposta em formato de json, utilizando para isso uma ação "GET". Retornando um objeto da classe Filme, que vai conter um atributo com o nome do filme.</p>
    <details>
    <summary>Serviço que consome a URL Https</summary>
    <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/servicoGetFilme.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> Esse serviço é chamado por pelo método recommendMovie() na classe principal, tendo seu resultado atribuído a um objeto da classe Filme. Utiliazamos esse resposta como parâmetro para um intent com ação de pesquisa na Web, assim levará o usuário para mais informações sobre o filme que a URL recomenda.</p>
    <details>
    <summary>Método recommendMovie()</summary>
    <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/recommendMovie.png" width="800px;" alt=""/>
  </details>
  
  
  <h2 style="font-family:roboto;"> Aprendizados Efetivos :book:</h2>   
  <ul>
  <li>Metodologia Scrum:
  <ul>
    <li>Organização e acompanhamento constante do desenvolvimento das tarefas pela equipe.</li>   
    </ul></li>
  <li>Desenvolvimento Android Nativo:
  <ul>
    <li>Criação e configuração do ambiente no Android Studio;</li> 
    <li>Consumir API Https;</li>
    <li>Método para reconhecimento de comandos por voz;</li> 
    <li>Ações nativas android chamadas por comando de voz.</li>
    </ul></li>
    </ul>
    
---
  
  <h2 align="center"> API 2º Semestre</h2>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> A empresa TecSUS requisitou o desenvolvimento de um software que tem por objetivo facilitar a digitação por parte da sua equipe para as contas de água e luz. O software oferece uma maior facilidade para seus usuários, automatizando processos e diminuindo o tempo de cadastro, além da prevenção de erros por parte dos digitadores e gerando um relatório sobre o consumo e custos de água e luz de cada cliente. Para mais informações sobre o projeto, acesse: <a href="https://github.com/GabrielSG20/Projeto_Integrador_2-Sem2020">Cadastro de Contas</a>.</p>
  
  <h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
   
  <ul>
  <li><a href="https://www.java.com/pt_BR/">Java</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Linguagem de programação utilizada para o desenvolvimento Back-End do sistema, apresenta como principais características: Portabilidade, Robustez, Segurança, Orientação a Objetos, Dinâmica e Alto Desempenho. Foi um requisito técnico solicitado pelo cliente.</p></li>
  </ul></li>
  <li><a href="https://openjfx.io/">JavaFX</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Plataforma de software multimídia utilizada para criação de interfaces gráficas, utilizando a linguagem Java. </p></li>
  </ul></li>
   <li><a href="https://www.mysql.com/">MySQL</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Sistema de gerenciamento de banco de dados utilizado para criação e manipulação de bases de dados, onde eram armazenadas as informações do software.</p></li>
  </ul></li>
  <li><a href="https://www.gitpod.io/">Gitpod</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Ambiente de desenvolvimento em nuvem utilizado para elaboração de aplicações Web ou Desktop em diversas linguagens de programação.</p></li>
  </ul></li>
  <li><a href="https://trello.com/https://trello.com">Trello</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Foi utilizado como ferramenta do método Scrum para distribuição das atividades do grupo e priorização das demandas. Possibilitando realizar o planejamento das sprints, sendo capaz de registrar o progresso da equipe e do projeto, facilitando o desenvolvimento e acompanhamento da realização de tarefas. </p></li>
  </ul></li>

  </ul>
  
  <h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  
  <h3> Atribuições como Desenvolvedor Back-end</h3>
  
  <h3> Atribuições como Scrum Master</h3>
  <p align="justify" style="font-family:roboto;"> As atribuições como Scrum Master da equipe são pertinentes a realizar um bom planejamento e organização das ações do grupo no decorrer das Sprints. No início do projeto foi realizada uma reunião para definir nosso principal meio de comunicação e a ferramenta para monitoramento de tarefas, assim decidimos utilizar, respectivamente, o Discord e o Trello. Como Master da equipe, fiquei responsável por acompanhar e analizar o progresso do grupo nesses softwares, de modo a observar se todos os integrantes estavam participando das Weekly Meatings e se apresentavam alguma dificuldade com a evolução das tarefas, logo atuando da melhor maneira de acordo com a situação.</p>
  <p align="justify" style="font-family:roboto;"> Após a apresentação do problema por parte do cliente, nos reunimos para a elaboração de um Backlog conciso com as necessidades do cliente. Obtendo como resultado final desse processo as User Stories que compõe o Product Backlog e a descrição da experiência do usuário com o produto, além de promover um ótimo entendimento das regras de negócio e os primeiros questionamentos para o cliente. Com esse alinhamento inicial finalizado, as User Stories foram divididas entre as 4 Sprints do projeto, destarte tive a função de quebrar essas histórias em tarefas menores e mais objetivas, para um melhor desenvolvimento do que foi planejado, e também delegar essas tasks entre os integrantes da equipe. O que pode ser observado na imagem exemplo abaixo.</p>
  <details>
  <summary>Demonstração da Organização de uma Sprint no Trello</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/TrelloAPI2.png" width="1000px;" alt=""/>
  </details>
  
  <h2 style="font-family:roboto;"> Aprendizados Efetivos :book:</h2>   
  <ul>
  <li>Metodologia Scrum:
  <ul>
    <li>Quebra das User Stories da Sprint em Tasks objetivas;</li>
    <li>Organização e acompanhamento constante do desenvolvimento das tarefas pela equipe.</li>   
    </ul></li>
  <li>Padrão de projetos DAO:
  <ul>
    <li>Conexão com Banco de Dados Mysql.</li>
    </ul></li>
    </ul>
    
---
    
  <h2 align="center"> API 3º Semestre</h2>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> Para otimizar a criação e melhorar o controle na documentação de aeronaves, a empresa parceira solicitou a equipe airPLAN o desenvolvimento de uma aplicação que automatize e aperfeiçoe a forma de armazenar e gerar documentos de maneira intuitiva e eficaz. O objetivo é desenvolver uma aplicação que integre três APIs independentes. Além disso, as ferramentas necessitam manter, customizar e versionar partes de arquivos em PDF, utilizando regras de negócio específicas para gerar documentos finais que dispõe as partes selecionadas.Para mais informações sobre o projeto, acesse: <a href="https://github.com/GabrielSG20/Projeto_Integrador_3BD-1Sem2021">AirPlan</a>.</p>
  
  <h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
   
  <ul>
  <li><a href="https://www.java.com/pt_BR/">Java</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Linguagem de programação utilizada para o desenvolvimento Back-End do sistema, apresenta como principais características: Portabilidade, Robustez, Segurança, Orientação a Objetos, Dinâmica e Alto Desempenho. Foi um requisito técnico solicitado pelo cliente.</p></li>
  </ul></li>
  <li><a href="https://spring.io/">Spring Boot</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> É um framework open source para Java, aplicado para facilitar a configuração e gerenciamento das dependências do projeto. Logo melhorando a produtividade e agilidade no processo de desenvolvimnto da aplicação.</p></li>
  </ul></li>
  <li><a href="https://www.thymeleaf.org/">Thymeleaf</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Foi utilizado no desenvolvimento Front-End para comunicação com a API Rest elaborada no Back-End. </p></li>
  </ul></li>
   <li><a href="https://www.mysql.com/">MySQL</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Sistema de gerenciamento de banco de dados utilizado para criação e manipulação de bases de dados, onde eram armazenadas as informações do software.</p></li>
  </ul></li>
  <li><a href="https://trello.com/https://trello.com">Trello</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Foi utilizado como ferramenta do método Scrum para distribuição das atividades do grupo e priorização das demandas. Possibilitando realizar o planejamento das sprints, sendo capaz de registrar o progresso da equipe e do projeto, facilitando o desenvolvimento e acompanhamento da realização de tarefas. </p></li>
  </ul></li>

  </ul>
  
  <h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  
  <h3> Atribuições como Desenvolvedor Back-end</h3>
  <p align="justify" style="font-family:roboto;"> Como Desenvolvedor Back-End, as atribuições foram relacionadas com a elaboração da lógica do sistema web planejado, tendo em vista as regras de negócio propostas pelo cliente. Criando os Endpoints que serão utilizados na interação com o Front-End, obtendo uma solução completa com todas as funcionalidades necessárias. Como demonstrado no tópico de Tecnologias Adotadas, foi utilizado Java com a framework Spring Boot para o desenvolvimento Back-End, portanto os próximos parágrafos irão descrever a minha experiência em contribuir com a lógica do projeto.</p>
  
  <p align="justify" style="font-family:roboto;"> O primeiro passo foi a configuração do ambiente que iríamos utilizar. A fizemos pelo <a href="https://start.spring.io/">Sprint Initializr</a>, o estruturando com Spring Boot 2.5.4, Java 8 e Maven. Logo, adicionamos todas as dependências necessárias no arquivo POM.xml, sendo as mais importantes: o driver de conexão com o Banco de Dados Oracle (mysql-connector-java), o JPA (spring-boot-starter-data-jpa), o Spring Boot Starter Web (spring-boot-starter-web) e o Thymeleaf (spring-boot-starter-thymeleaf). Como mostra a imagem a seguir.</p>
  <details>
  <summary>POM.xml do Projeto</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/Pom3Sem.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> Com isso finalizado e versionado no GitHub, focamos em decidir a Arquitetura e padrões de projetos que implementaríamos. Logo, optamos pela arquitetura Modelo-Visão-Controle (MVC), em que separamos o sistema em componentes interligados que são essenciais para uma melhora na conexão entre as camadas de dados, lógica de negócio e iteração com o usuário.</p>
  <details>
  <summary>Lógica Arquitetural MVC</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/DiagramaArq.png" width="500px;" alt=""/>
  </details>
  
  <ul>
  <li> Model: são representações das tabelas do Banco de Dados MySQL. Resultando em uma melhor validação dos dados e facilitação com consultas, inserções e atualizações na Database.
    <details>
  <summary>Entidade Model</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/modelAPI2.png" width="800px;" alt=""/>
  </details>
  </li>
    
  <li> Repositories: são interfaces que tem como função serem camadas de acesso a dados. Eles extendem o JpaRepository, portanto há um melhor e mais fácil acesso aos métodos de manipulação dos dados na Database, sendo inserção (save), consulta (listAll), atualização (save) e deleção (deleteById) os que utilizamos no desenvolvimento. Além de permitirem realizar comandos SQL customizados de acordo com a necessidade da funcionalidade.
  <details>
  <summary>Repository</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/RepositoryAPI2.png" width="800px;" alt=""/>
  </details>
  </li>
    
  <li> Services: são classes que concentram os métodos do Repository, visto que tem essa interface injetada com a anotação @Autowired. Sendo adicionados neles a lógica essencial para regra de negócio imposta pelo cliente, além de contribuirem muito para organização dos métodos utilizados pela interface.
  <details>
  <summary>Service</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/ServiceAPI2.png" width="800px;" alt=""/>
  </details>
  </li>
    
  <li> Controllers: são as classes onde se encontram os Endpoints do Back-End que serão utilizados para interação com o Front-End, isso corre pela chamada de rotas presentes em seus métodos, pela anotação @RequestMapping("/rota-exemplo"). Ademais, contém os Services necessários injetados com a anotação @Autowired e utiliza das chamadas dos métodos dessas classes para realização da lógica desenvolvida.
  <details>
  <summary>Controller</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/ControllerAPI2.png" width="800px;" alt=""/>
  </details>
  </li>
  </ul>
  
  <p align="justify" style="font-family:roboto;"> Foi implementado o padrão de projeto Proxy, uma vez que controlamos o acesso aos objetos nas requisições com as anotações do Spring Boot. Além do uso do padrão Facade, aplicado nos Repositories do sistema, no qual é uma interface que simplifica as funcionalidades das classes da Java Persistence API (JPA).</p>
  <details>
  <summary>Padrão de Projeto Proxy</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/PadraoProxy.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> A seguir foram configuradas as Properties, na qual foi aplicada a conexão com a Base de Dados MySQL. Além de declarar: o driver utilizado (com.mysql.cj.jdbc.Driver), a versão da linguagem do Banco (org.hibernate.dialect.MySQL8Dialect) e a porta que será rodado o serviço (PORT:8080).</p>
  <details>
  <summary>Properties</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/PropertiesAPI2.png" width="800px;" alt=""/>
  </details>
  
  <h3> Atribuições como Scrum Master</h3>
  <p align="justify" style="font-family:roboto;"> As atribuições como Scrum Master da equipe são pertinentes a realizar um bom planejamento e organização das ações do grupo no decorrer das Sprints. No início do projeto foi realizada uma reunião para definir nosso principal meio de comunicação e a ferramenta para monitoramento de tarefas, assim decidimos utilizar, respectivamente, o Discord e o Trello. Como Master da equipe, fiquei responsável por acompanhar e analizar o progresso do grupo nesses softwares, de modo a observar se todos os integrantes estavam participando das Weekly Meatings e se apresentavam alguma dificuldade com a evolução das tarefas, logo atuando da melhor maneira de acordo com a situação.</p>
  <p align="justify" style="font-family:roboto;"> Após a apresentação do problema por parte do cliente, nos reunimos para a elaboração de um Backlog conciso com as necessidades do cliente. Obtendo como resultado final desse processo as User Stories que compõe o Product Backlog e a descrição da experiência do usuário com o produto, além de promover um ótimo entendimento das regras de negócio e os primeiros questionamentos para o cliente. Com esse alinhamento inicial finalizado, as User Stories foram divididas entre as 4 Sprints do projeto, destarte tive a função de quebrar essas histórias em tarefas menores e mais objetivas, para um melhor desenvolvimento do que foi planejado, e também delegar essas tasks entre os integrantes da equipe. O que pode ser observado na imagem exemplo abaixo.</p>
  <details>
  <summary>Demonstração da Organização de uma Sprint no Trello</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/TrelloAPI3.png" width="1000px;" alt=""/>
  </details>
  
  
 <h2 style="font-family:roboto;"> Aprendizados Efetivos :book:</h2>   
  <ul>
  <li>Metodologia Scrum:
  <ul>
    <li>Quebra das User Stories da Sprint em Tasks objetivas;</li>
    <li>Organização e acompanhamento constante do desenvolvimento das tarefas pela equipe.</li>   
    </ul></li>
  <li>Framework Spring Boot:
  <ul>
    <li>Configuração do ambiente;</li> 
    <li>Arquitetura Modelo-Visão-Controle (MVC);</li>
    <li>Desenvolvimento dos Endpoints para chamada do Front-End;</li> 
    <li>Mapeamento das tabelas da Base de Dados;</li>
    <li>Conexão com Banco de Dados Mysql.</li>
    </ul></li>
    </ul>
    
---
  
  <h2 align="center"> API 4º Semestre</h2>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> :calendar: <b>#VEMPRACASA</b> é uma parceria entre a <a href="https://www.oracle.com/br/index.html">Oracle</a> e a FATEC São José dos Campos com a finalidade de desenvolvimento de um sistema para realização de agendamentos de eventos nos espaços da Casa Oracle, seguindo as normas vigentes de ocupação por conta da Pandemia do Coronavírus.</p>
  <p align="justify" style="font-family:roboto;"> O sistema foi planejado com uma série de funcionalidades com objetivo de deixar mais intuitivo e produtivo o cadastro e participação de eventos nos dois espaços disponíveis (Open Space e Lounge on Hall). Essas funções estão divididas entre os tipos de usuários do sistema, que são: Admin, Organizador, Interno e Externo.</p>
  <p align="justify" style="font-family:roboto;"> O Admin é quem tem o controle sobre a aprovação ou recusa de eventos no calendário, podendo priorizar os que estiverem marcados na mesma data, hora e local, além de ter acesso à relatórios sobre os eventos realizados e conseguindo cadastrar novos fornecedores (empresas terceirizadas) para apoio aos organizadores. O Usuário Organizador poderá agendar eventos nos espaços diponíveis preenchendo as informações necessárias, podendo criar uma lista de convidados adicionando os e-mails dos remententes no cadastro, além de ser capaz de visualizar os contatos dos fornecedores disponíveis. O Interno conseguirá se inscrever para eventos abertos ao público em geral ou os quais foi convidado, também tem acesso a solicitar permissão para se tornar Oraganizador, visto que é obrigatório esse usuário ter um e-mail Oracle. Já o Externo se destina ao público em geral que deseja participar dos eventos abertos, sendo capaz de apenas visualizar o calendário e se inscrever nas palestras de seu interesse.</p>
    <p align="justify" style="font-family:roboto;">Nessa documentação será abordado o ponto de vista do Scrum Master/Desenvolvedor Back-End da Equipe Sight Future, demonstrando minhas constribuições no planejamento e desenvolvimento do API 4º Semestre. Para mais informações sobre o projeto, acesse: <a href="https://github.com/GabrielSG20/API4Sem2021">#VEMPRACASA</a>.</p>
  
  
  <h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
   
  <ul>
  <li><a href="https://www.java.com/pt_BR/">Java</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Linguagem de programação utilizada para o desenvolvimento Back-End do sistema, apresenta como principais características: Portabilidade, Robustez, Segurança, Orientação a Objetos, Dinâmica e Alto Desempenho. Foi um requisito técnico solicitado pelo cliente.</p></li>
  </ul></li>
    
  <li><a href="https://spring.io/">Spring Boot</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> É um framework open source para Java, aplicado para facilitar a configuração e gerenciamento das dependências do projeto. Logo melhorando a produtividade e agilidade no processo de desenvolvimnto da aplicação.</p></li>
  </ul></li>
    
  <li><a href="https://angular.io/">Angular</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> O Front-End do projeto foi realizado com Angular, uma plataforma para desenvolvimento de aplicações web com um código open source com base em TypeScript, foi escolhido pela equipe pela possibilidade de criação de páginas dinâmicas e otimização de trabalho com reescrita de código.</p></li>
  </ul></li>
    
  <li><a href="https://miragejs.com/">MirageJS</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> É uma biblioteca de simulação de API que permite construir, testar e compartilhar um aplicativo JavaScript funcional completo sem ter que depender de nenhum Back-End. Foi empregado para realização de testes das telas do Front-End, no momento em que não existia conexão com o Back-End.</p></li>
  </ul></li>
      
  <li><a href="https://www.oracle.com/tools/downloads/sqldev-downloads.html">Oracle SQL Developer</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Na parte de armazenamento de dados, foi utilizado o Oracle Database 12c, um SGBD relacional, escolhido por atender todas as necessidades do projeto e ser uma ferramenta da empresa parceira. Para trabalhar com scripts SQL nessa Base de Dados selecionada, usamos o Oracle SQL Developer, um ambiente de desenvolvimento integrado com o Bancos de Dados Oracle.</p></li>
  </ul></li>
        
  <li><a href="https://www.figma.com/">Figma</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> É uma ferramenta para projetos UI com excelentes recursos de Design, Prototipagem, Colaboração, Plug-in de Sistema de Projeto, entre outros. Foi empregado pela nossa equipe para realização da metodologia Product Backlog Building (PBB) e criação das Wireframes.</p></li>
  </ul></li>
          
  <li><a href="https://vempracasa.atlassian.net/">Jira</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> Foi utilizado como ferramenta do método Scrum para distribuição das atividades do grupo e priorização das demandas. Possibilitando realizar o planejamento das sprints, sendo capaz de registrar o progresso da equipe e do projeto, facilitando o desenvolvimento e acompanhamento da realização de tarefas.</p></li>
  </ul></li>
       
  <li><a href="https://www.oracle.com/br/cloud/">Oracle Cloud</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> É um serviço de computação em nuvem oferecido pela Oracle Corporation. Foi usado para o deploy do Back-End e Banco de Dados Oracle do projeto.</p></li>
  </ul></li>
       
  <li><a href="https://www.heroku.com/platform">Heroku</a>:
  <ul>
    <li><p align="justify" style="font-family:roboto;"> É uma plataforma em nuvem com um serviço que suporta várias linguagens de programação, nela foi realizado o deploy do Front-End da aplicação.</p></li>
  </ul></li>
  </ul>
 
  
  <h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  
  <h3> Atribuições como Desenvolvedor Back-end</h3>
  <p align="justify" style="font-family:roboto;"> Como Desenvolvedor Back-End, as atribuições foram relacionadas com a elaboração da lógica do sistema web planejado, tendo em vista as regras de negócio propostas pelo cliente. Criando os Endpoints que serão utilizados na interação com o Front-End, obtendo uma solução completa com todas as funcionalidades necessárias. Como demonstrado no tópico de Tecnologias Adotadas, foi utilizado Java com a framework Spring Boot para o desenvolvimento Back-End, portanto os próximos parágrafos irão descrever a minha experiência em contribuir com a lógica do projeto.</p>
  
  <p align="justify" style="font-family:roboto;"> O primeiro passo foi a configuração do ambiente que iríamos utilizar. A fizemos pelo <a href="https://start.spring.io/">Sprint Initializr</a>, o estruturando com Spring Boot 2.5.4, Java 8 e Maven. Logo, adicionamos todas as dependências necessárias no arquivo POM.xml, sendo as mais importantes: o driver de conexão com o Banco de Dados Oracle (ojdbc8), o JPA (spring-boot-starter-data-jpa) e o Spring Boot Starter Web (spring-boot-starter-web). Como mostra a imagem a seguir.</p>
  <details>
  <summary>POM.xml do Projeto</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/Pom.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> Com isso finalizado e versionado no GitHub, focamos em decidir a Arquitetura e padrões de projetos que implementaríamos. Logo, optamos pela arquitetura Modelo-Visão-Controle (MVC), em que separamos o sistema em componentes interligados que são essenciais para uma melhora na conexão entre as camadas de dados, lógica de negócio e iteração com o usuário.</p>
  <details>
  <summary>Lógica Arquitetural MVC</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/DiagramaArq.png" width="500px;" alt=""/>
  </details>
  
  <ul>
  <li> Model: são representações das tabelas do Banco de Dados Oracle, tendo seus campos e relações mapeadas pelo Hibernate. Resultando em uma melhor validação dos dados e facilitação com consultas, inserções e atualizações na Database.
    <details>
  <summary>Entidade Model</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/Model-1.png" width="800px;" alt=""/>
  </details>
  <details>
  <summary>Relações ManyToMany e ManyToOne Mapeadas</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/Model-2.png" width="800px;" alt=""/>
  </details>
  </li>
    
  <li> Repositories: são interfaces que tem como função serem camadas de acesso a dados. Eles extendem o JpaRepository, portanto há um melhor e mais fácil acesso aos métodos de manipulação dos dados na Database, sendo inserção (save), consulta (listAll), atualização (save) e deleção (deleteById) os que utilizamos no desenvolvimento. Além de permitirem realizar comandos SQL customizados de acordo com a necessidade da funcionalidade.
  <details>
  <summary>Repository</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/Repository.png" width="800px;" alt=""/>
  </details>
  </li>
    
  <li> Services: são classes que concentram os métodos do Repository, visto que tem essa interface injetada com a anotação @Autowired. Sendo adicionados neles a lógica essencial para regra de negócio imposta pelo cliente, como por exemplo o envio de e-mails, além de contribuirem muito para organização dos métodos utilizados pela interface.
  <details>
  <summary>Service</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/Service.png" width="800px;" alt=""/>
  </details>
  </li>
    
  <li> Controllers: são as classes onde se encontram os Endpoints do Back-End que serão utilizados para interação com o Front-End, isso corre pela chamada de rotas presentes em seus métodos, pela anotação @RequestMapping("/rota-exemplo"). Ademais, contém os Services necessários injetados com a anotação @Autowired e utiliza das chamadas dos métodos dessas classes para realização da lógica desenvolvida.
  <details>
  <summary>Controller</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/Controller.png" width="800px;" alt=""/>
  </details>
  </li>
  </ul>
  
  <p align="justify" style="font-family:roboto;"> Ademais, utilizarmos arquitetura REST, visto que a comunicação entre as aplicações ocorre com requisições HTTP, podendo ser perceptível pelas rotas nos controllers demonstradas nos parágrafos anteriores. Nesse ponto também foi implementado o padrão de projeto Proxy, uma vez que controlamos o acesso aos objetos nas requisições com as anotações do Spring Boot. Além do uso do padrão Facade, aplicado nos Repositories do sistema, no qual é uma interface que simplifica as funcionalidades das classes da Java Persistence API (JPA).</p>
  <details>
  <summary>Padrão de Projeto Proxy</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/PadraoProxy.png" width="800px;" alt=""/>
  </details>
  
   <p align="justify" style="font-family:roboto;"> Após explicada a estrura empregada no projeto, foi necessário realizar uma configuração de Cors, ao passo que verificam a real origem, métodos HTTP e cabeçalhos de uma determinada solicitação enviada para o Back-End. Sendo fundamental para conexão com o Front-End, porque permite que a rota utilizada no Angular consiga fazer requisições e receber suas respostas.</p>
  <details>
  <summary>Configuração dos Cors</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/Config-Cors.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> A seguir foram configuradas as Properties, na qual foi aplicada a conexão com a Base de Dados Oracle que está em
  nuvem no Oracle Cloud, por meio do sistema de Wallet. Além de declarar: o driver utilizado (oracle.jdbc.OracleDriver), a versão da linguagem do Banco (Oracle12cDialect), a maneira que o hibernate vai ler os Models (validate) e a porta que será rodado o serviço (PORT:8080).</p>
  <details>
  <summary>Properties</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/Properties-VPC.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> Por fim, colaborei com o deploy do Front-End no Heroku, por meio do método manual usando uma branch do GitHub do projeto. Com isso o sistema ficou 100% hospedado em nuvem e disponível pelo seguinte link: <a href="http://vempracasa.herokuapp.com/">#VEMPRACASA</a></p>
  <details>
  <summary>Heroku</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/Heroku.png" width="1000px;" alt=""/>
  </details>
  
  <h3> Atribuições como Scrum Master</h3>
  <p align="justify" style="font-family:roboto;"> As atribuições como Scrum Master da Equipe Sight Future são pertinentes a realizar um bom planejamento e organização das ações do grupo no decorrer das Sprints. No início do projeto foi realizada uma reunião para definir nosso principal meio de comunicação e a ferramenta para monitoramento de tarefas, assim decidimos utilizar, respectivamente, o Discord e o Jira. Como Master da equipe, fiquei responsável por acompanhar e analizar o progresso do grupo nesses softwares, de modo a observar se todos os integrantes estavam participando das Weekly Meatings e se apresentavam alguma dificuldade com a evolução das tarefas, logo atuando da melhor maneira de acordo com a situação.</p>
  <p align="justify" style="font-family:roboto;"> Após a apresentação do problema por parte do cliente, utilizamos a metodologia Product Backlog Building (<a href="https://www.caroli.org/livro/pbb/">AGUIAR; CAROLI, 2021</a>) para a elaboração de um Backlog conciso com as necessidades do cliente. Obtendo como resultado final desse processo as User Stories que compõe o Product Backlog e a descrição da experiência do usuário com o produto, além de promover um ótimo entendimento das regras de negócio e os primeiros questionamentos para o cliente. Com esse alinhamento inicial finalizado, as User Stories foram divididas entre as 4 Sprints do projeto, destarte tive a função de quebrar essas histórias em tarefas menores e mais objetivas, para um melhor desenvolvimento do que foi planejado, e também delegar essas tasks entre os integrantes da equipe. O que pode ser observado na imagem exemplo abaixo.</p>
  <details>
  <summary>Demonstração da Organização de uma Sprint no Jira</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Bertoti/blob/main/TG1/images/Jira.png" width="1000px;" alt=""/>
  </details>
  
   
  <h2 style="font-family:roboto;"> Aprendizados Efetivos :book:</h2>   
  <ul>
  <li>Metodologia Scrum:
  <ul>
    <li>Criação do Product Backlog pela metodologia Product Backlog Building (PBB);</li>
    <li>Quebra das User Stories da Sprint em Tasks objetivas;</li>
    <li>Organização e acompanhamento constante do desenvolvimento das tarefas pela equipe.</li>   
    </ul></li>
  <li>Framework Spring Boot:
  <ul>
    <li>Configuração do ambiente;</li> 
    <li>Arquitetura Modelo-Visão-Controle (MVC);</li>
    <li>Desenvolvimento dos Endpoints para chamada do Front-End;</li> 
    <li>Mapeamento das tabelas e relações da Base de Dados com Hibernate;</li>
    <li>Conexão com Banco de Dados Oracle hospedado em nuvem no Oracle Cloud, por meio da Wallet.</li>
    </ul></li>
  <li>Deploy em Nuvem:
  <ul>
    <li>Configuração do código para deploy;</li>
    <li>Deploy no Heroku, por meio do método Manual usando uma branch do GitHub.</li>   
    </ul></li>
    </ul>
    
---

</body>
</html>
