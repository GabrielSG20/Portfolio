<html>
<body>
  
 <h1 align="center"> API 4º Semestre Banco de Dados</h1>
  
  <p align="center">
 <a href="#-resumo-do-projeto-clipboard"> Resumo do Projeto</a> •
 <a href="#-tecnologias-adotadas-computer">Tecnologias Adotadas</a> •
 <a href="#-contribuições-individuais-dart">Contribuições Individuais</a> •
 <a href="#-aprendizados-efetivos-book">Aprendizados Efetivos</a>
</p>
  
  ---
  
  <h2> Autor :necktie: </h2>
  <table align="center">
   <tr>
    <td align="center"><a href="https://www.linkedin.com/in/gabrielsoaresgoncalves/"><img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/GabrielSoares.jfif" width="200px;" alt=""/><br/><b>Gabriel Soares</b></a>
      <br/>
      Scrum Master/Developer
     </td>
   </tr>
  </table>

 ---
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> :calendar: <b>#VEMPRACASA</b> é uma parceria entre a <a href="https://www.oracle.com/br/index.html">Oracle</a> e a FATEC São José dos Campos com a finalidade de desenvolvimento de um sistema para realização de agendamentos de eventos nos espaços da Casa Oracle, seguindo as normas vigentes de ocupação por conta da Pandemia do Coronavírus.</p>
  <p align="justify" style="font-family:roboto;"> O sistema foi planejado com uma série de funcionalidades com objetivo de deixar mais intuitivo e produtivo o cadastro e participação de eventos nos dois espaços disponíveis (Open Space e Lounge on Hall). Essas funções estão divididas entre os tipos de usuários do sistema, que são: Admin, Organizador, Interno e Externo.</p>
  <p align="justify" style="font-family:roboto;"> O Admin é quem tem o controle sobre a aprovação ou recusa de eventos no calendário, podendo priorizar os que estiverem marcados na mesma data, hora e local, além de ter acesso à relatórios sobre os eventos realizados e conseguindo cadastrar novos fornecedores (empresas terceirizadas) para apoio aos organizadores. O Usuário Organizador poderá agendar eventos nos espaços diponíveis preenchendo as informações necessárias, podendo criar uma lista de convidados adicionando os e-mails dos remententes no cadastro, além de ser capaz de visualizar os contatos dos fornecedores disponíveis. O Interno conseguirá se inscrever para eventos abertos ao público em geral ou os quais foi convidado, também tem acesso a solicitar permissão para se tornar Oraganizador, visto que é obrigatório esse usuário ter um e-mail Oracle. Já o Externo se destina ao público em geral que deseja participar dos eventos abertos, sendo capaz de apenas visualizar o calendário e se inscrever nas palestras de seu interesse.</p>
    <p align="justify" style="font-family:roboto;">Nessa documentação será abordado o ponto de vista do Scrum Master/Desenvolvedor Back-End da Equipe Sight Future, demonstrando minhas constribuições no planejamento e desenvolvimento do API 4º Semestre. Para mais informações sobre o projeto, acesse: <a href="https://github.com/GabrielSG20/API4Sem2021">#VEMPRACASA</a>.</p>
  
  ---
  
  <h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
   
  * [Java](https://www.java.com/pt_BR/)
  * [Spring Boot](https://spring.io/)
  * [JavaScript](https://www.javascript.com/)
  * [Angular](https://angular.io/)
  * [Oracle SQL Developer](https://www.oracle.com/tools/downloads/sqldev-downloads.html)
  * [Figma](https://www.figma.com/)
  * [Jira](https://vempracasa.atlassian.net/) 
  * [Oracle Cloud](https://www.oracle.com/br/cloud/) 
  * [Heroku](https://www.heroku.com/platform) 
  
  ---
  
  <h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  <h3> Atribuições como Scrum Master</h3>
  <p align="justify" style="font-family:roboto;"> As atribuições como Scrum Master da Equipe Sight Future são pertinentes a realizar um bom planejamento e organização das ações do grupo no decorrer das Sprints. No início do projeto foi realizada uma reunião para definir nosso principal meio de comunicação e a ferramenta para monitoramento de tarefas, assim decidimos utilizar, respectivamente, o Discord e o Jira. Como Master da equipe, fiquei responsável por acompanhar e analizar o progresso do grupo nesses softwares, de modo a observar se todos os integrantes estavam participando das Weekly Meatings e se apresentavam alguma dificuldade com a evolução das tarefas, logo atuando da melhor maneira de acordo com a situação.</p>
  <p align="justify" style="font-family:roboto;"> Após a apresentação do problema por parte do cliente, utilizamos a metodologia Product Backlog Building (<a href="https://www.caroli.org/livro/pbb/">AGUIAR; CAROLI, 2021</a>) para a elaboração de um Backlog conciso com as necessidades do cliente. Obtendo como resultado final desse processo as User Stories que compõe o Product Backlog e a descrição da experiência do usuário com o produto, além de promover um ótimo entendimento das regras de negócio e os primeiros questionamentos para o cliente. Com esse alinhamento inicial finalizado, as User Stories foram divididas entre as 4 Sprints do projeto, destarte tive a função de quebrar essas histórias em tarefas menores e mais objetivas, para um melhor desenvolvimento do que foi planejado, e também delegar essas tasks entre os integrantes da equipe. O que pode ser observado na imagem exemplo abaixo.</p>
  <details>
  <summary>Demonstração da Organização de uma Sprint no Jira</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/Jira.png" width="1000px;" alt=""/>
  </details>
  
  <h3> Atribuições como Desenvolvedor Back-End</h3>
  <p align="justify" style="font-family:roboto;"> Como Desenvolvedor Back-End, as atribuições foram relacionadas com a elaboração da lógica do sistema web planejado, tendo em vista as regras de negócio propostas pelo cliente. Criando os Endpoints que serão utilizados na interação com o Front-End, obtendo uma solução completa com todas as funcionalidades necessárias. Como demonstrado no tópico de Tecnologias Adotadas, foi utilizado Java com a framework Spring Boot para o desenvolvimento Back-End, portanto os próximos parágrafos irão descrever a minha experiência em contribuir com a lógica do projeto.</p>
  
  <p align="justify" style="font-family:roboto;"> O primeiro passo foi a configuração do ambiente que iríamos utilizar. A fizemos pelo <a href="https://start.spring.io/">Sprint Initializr</a>, o estruturando com Spring Boot 2.5.4, Java 8 e Maven. Logo, adicionamos todas as dependências necessárias no arquivo POM.xml, sendo as mais importantes: o driver de conexão com o Banco de Dados Oracle (ojdbc8), o JPA (spring-boot-starter-data-jpa) e o Spring Boot Starter Web (spring-boot-starter-web). Como mostra a imagem a seguir.</p>
  <details>
  <summary>POM.xml do Projeto</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/Pom.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> Com isso finalizado e versionado no GitHub, decidimos qual seria a Arquitetura a se empregar com o Spring Boot e chegamos no seguinte resultado:</p>
  <details>
  <summary>Lógica Arquitetural</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/DiagramaArq.png" width="500px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> As Models são representações das tabelas do Banco de Dados Oracle, tendo seus campos e relações mapeadas pelo Hibernate. Resultando em uma melhor validação dos dados e facilitação com consultas, inserções e atualizações na Database.</p>
  <details>
  <summary>Entidade Model</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/Model-1.png" width="800px;" alt=""/>
  </details>
  <details>
  <summary>Relações ManyToMany e ManyToOne Mapeadas</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/Model-2.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> Os Repositories são interfaces que tem como função serem camadas de acesso a dados. Eles extendem o JpaRepository, portanto há um melhor e mais fácil acesso aos métodos de manipulação dos dados na Database, sendo inserção (save), consulta (listAll), atualização (save) e deleção (deleteById) os que utilizamos no desenvolvimento. Além de permitirem realizar comandos SQL customizados de acordo com a necessidade da funcionalidade.</p>
  <details>
  <summary>Repository</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/Repository.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> Os Services são classes que concentram os métodos do Repository, visto que tem essa interface injetada com a anotação @Autowired. Sendo adicionados neles a lógica essencial para regra de negócio imposta pelo cliente, como por exemplo o envio de e-mails, além de contribuirem muito para organização dos métodos utilizados pela interface.</p>
  <details>
  <summary>Service</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/Service.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> Os Controllers são as classes onde se encontram os Endpoints do Back-End que serão utilizados para interação com o Front-End, isso corre pela chamada de rotas presentes em seus métodos, pela anotação @RequestMapping("/rota-exemplo"). Ademais, contém os Services necessários injetados com a anotação @Autowired e utiliza das chamadas dos métodos dessas classes para realização da lógica desenvolvida.</p>
  <details>
  <summary>Controller</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/Controller.png" width="800px;" alt=""/>
  </details>
  
   <p align="justify" style="font-family:roboto;"> Após explicada a estrura aplicada no projeto, foi necessário realizar uma configuração de Cors, ao passo que verificam a real origem, métodos HTTP e cabeçalhos de uma determinada solicitação enviada para o Back-End. Sendo fundamental para conexão com o Front-End, ao passo que permite que a rota utilizada no Angular consiga fazer requisições e receber suas respostas.</p>
  <details>
  <summary>Configuração dos Cors</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/Config-Cors.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> A seguir foram configuradas as Properties, na qual foi aplicada a conexão com a Base de Dados Oracle que está em
  nuvem no Oracle Cloud, por meio do sistema de Wallet. Além de declarar: o driver utilizado (oracle.jdbc.OracleDriver), a versão da linguagem do Banco (Oracle12cDialect), a maneira que o hibernate vai ler os Models (validate) e a porta que será rodado o serviço (PORT:8080).</p>
  <details>
  <summary>Properties</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/Properties-VPC.png" width="800px;" alt=""/>
  </details>
  
  <p align="justify" style="font-family:roboto;"> Por fim, colaborei com o deploy do Front-End no Heroku, por meio do método manual usando uma branch do GitHub do projeto. Com isso o sistema ficou 100% hospedado em nuvem e disponível pelo seguinte link: <a href="http://vempracasa.herokuapp.com/">#VEMPRACASA</a></p>
  <details>
  <summary>Heroku</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/Heroku.png" width="1000px;" alt=""/>
  </details>
  
  ---
   
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
    <li>Arquitetura com Repository, Service, Model e Controller;</li>
    <li>Desenvolvimento dos Endpoints para chamada do Front-End;</li> 
    <li>Mapeamento das tabelas e relações da Base de Dados com Hibernate;</li>
    <li>Conexão com Banco de Dados Oracle hospedado em nuvem no Oracle Cloud, por meio da Wallet.</li>
    </ul></li>
  <li>Deploy em Nuvem:
  <ul>
    <li>Configuração do código para deploy;</li>
    <li>Deploy no Heroku, por meio do método Manual usando uma branch do GitHub.</li>   
    </ul></li>
  
  ---

</body>
</html>
