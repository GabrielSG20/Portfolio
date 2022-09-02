<html>
<body>
    
  <h1 align="center"> API 3º Semestre - 01/2021</h1>
    <a href="https://github.com/GabrielSG20/Projeto_Integrador_3BD-1Sem2021"><img src="https://img.shields.io/badge/GitHub-Repositório Projeto-181717?style=for-the-badge&logo=github"></a>

  <h2> Parceiro Acadêmico: <a href="https://embraer.com/">Embraer</a></h2>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> Para otimizar a criação e melhorar o controle na documentação de aeronaves, a empresa parceira solicitou a equipe airPLAN o desenvolvimento de uma aplicação que automatize e aperfeiçoe a forma de armazenar e gerar documentos de maneira intuitiva e eficaz. O objetivo é desenvolver uma aplicação que integre três APIs independentes. Além disso, as ferramentas necessitam manter, customizar e versionar partes de arquivos em PDF, utilizando regras de negócio específicas para gerar documentos finais que dispõe as partes selecionadas.</p>
  
  <h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
   
  <ul>
  <li><a href="https://www.java.com/pt_BR/">Java</a>:
    <p align="justify" style="font-family:roboto;"> Linguagem de programação utilizada para o desenvolvimento Back-End do sistema, apresenta como principais características: Portabilidade, Robustez, Segurança, Orientação a Objetos, Dinâmica e Alto Desempenho. Foi um requisito técnico solicitado pelo cliente.</p></li>

  <li><a href="https://spring.io/">Spring Boot</a>:
    <p align="justify" style="font-family:roboto;"> É um framework open source para Java, aplicado para facilitar a configuração e gerenciamento das dependências do projeto. Logo melhorando a produtividade e agilidade no processo de desenvolvimnto da aplicação.</p></li>

  <li><a href="https://www.thymeleaf.org/">Thymeleaf</a>:
    <p align="justify" style="font-family:roboto;"> Foi utilizado no desenvolvimento Front-End para comunicação com a API Rest elaborada no Back-End. </p></li>

   <li><a href="https://www.mysql.com/">MySQL</a>:
    <p align="justify" style="font-family:roboto;"> Sistema de gerenciamento de banco de dados utilizado para criação e manipulação de bases de dados, onde eram armazenadas as informações do software.</p></li>

  <li><a href="https://trello.com/https://trello.com">Trello</a>:
      <p align="justify" style="font-family:roboto;"> Foi utilizado como ferramenta do método Scrum para distribuição das atividades do grupo e priorização das demandas. Possibilitando realizar o planejamento das sprints, sendo capaz de registrar o progresso da equipe e do projeto, facilitando o desenvolvimento e acompanhamento da realização de tarefas. </p></li>

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
  
  
  <h2 style="font-family:roboto;"> Funcionamento :bulb:</h2>

   <div align="center">
     <video src="https://user-images.githubusercontent.com/61523979/188246553-3cc60141-ef9e-4a7c-8bda-cc97cb6241b8.mp4" controls="controls" style="max-rate: 730px;">
     </video>    
   </div>

  <h2 style="font-family:roboto;"> Aprendizados Efetivos :book:</h2>   
  <h3 align="center"> Hard Skills </h3>
  <table align="center">
    <tr>
      <th width="300px">Tecnologia/Metodologia</th>
      <th width="300px">Classificação</th>
    </tr>
    <tr>
      <td>Metodologia Scrum - Scrum Master</td>
      <td>★★★★★★☆☆☆☆</td>
    </tr>
    <tr>
      <td>Java</td>
      <td>★★★★★★☆☆☆☆</td>
    </tr>
    <tr>
      <td>Spring Boot</td>
      <td>★★★★★☆☆☆☆☆</td>
    </tr>
    <tr>
      <td>MySQL</td>
      <td>★★★★★★★☆☆☆</td>
    </tr>
     <tr>
      <td>GIT</td>
      <td>★★★★★★★☆☆☆</td>
    </tr>
  </table>
  
  <h3 align="center">Soft Skills</h3>
  <table align="center">
    <tr>
      <th width="300px">Habilidade</th>
      <th width="300px">Classificação</th>
    </tr>
    <tr>
      <td>Proatividade</td>
      <td>★★★★★★★☆☆☆</td>
    </tr>
    <tr>
      <td>Visão de Negócio</td>
      <td>★★★★★★☆☆☆☆</td>
    </tr>
    <tr>
      <td>Comunicação</td>
      <td>★★★★★★★☆☆☆</td>
    </tr>
    <tr>
      <td>Organização</td>
      <td>★★★★★★★☆☆☆</td>
    </tr>
    <tr>
      <td>Planejamento</td>
      <td>★★★★★★☆☆☆☆</td>
    </tr>
  </table>

</body>
</html>
