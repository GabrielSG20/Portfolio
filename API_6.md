<html>
<body>
  
  <h1 align="center"> API 6º Semestre - 02/2022</h1>
<a href="https://github.com/API6Sem22/API6Doc"><img src="https://img.shields.io/badge/GitHub-Repositório Projeto-181717?style=for-the-badge&logo=github"></a>

  <h2> Parceiro Acadêmico: <a href="https://www.domrock.net/">Dom Rock</a></h2>
  
  <h2 style="font-family:roboto;"> Resumo do Projeto :clipboard:</h2>
  
  <p align="justify" style="font-family:roboto;"> :chart_with_upwards_trend: Esse projeto é uma parceria entre a Dom Rock e FATEC São José dos Campos, com objetivo de desenvolver uma solução que permita o armazenamento, organização e visualização dos dados oferecidos por duas fontes distintas. A equipe D-end ofereceu uma ferramenta capaz de realizar o cruzamento dos dados provenientes de convênios médicos e seus clientes, com o intuito de identificar inconsistências no pagamento das faturas das duas fontes de dados e com isso definir o plano de ação para cada situação encontrada.</p>
 
  
  <h2 style="font-family:roboto;"> Tecnologias Adotadas :computer:</h2>
   
  <ul>
  <li><a href="https://www.microsoft.com/pt-br/sql-server/sql-server-downloads">Microsoft SQL Server</a>:
   <p align="justify" style="font-family:roboto;"> Um sistema gerenciador de banco de dados relacional, utilizado para gerenciar o banco de dados que armazena as informações que serão exibidas no PowerBI.</p></li>
  
  <li><a href="https://powerbi.microsoft.com/pt-br/">Power BI</a>:
   <p align="justify" style="font-family:roboto;"> Um serviço de análise de negócios e análise de dados. Utilizado no projeto para criação de telas que permitem a visualização dos dados, demonstrando as informações em forma gráfica.</p></li>
  
  <li><a href="https://azure.microsoft.com/pt-br/services/sql-database/campaign/#overview">Microsoft Azure</a>:
   <p align="justify" style="font-family:roboto;"> É uma plataforma destinada à execução de aplicativos e serviços, baseada nos conceitos da computação em nuvem. Foi utilizado para deploy do banco de dados SQL Server.</p></li>
  
  <li><a href="https://vertabelo.com/">Vertabelo</a>:
   <p align="justify" style="font-family:roboto;"> Uma ferramenta empregada para modelagem e documentação do banco de dado SQL Server.</p></li>
        
  <li><a href="https://www.figma.com/">Figma</a>:
  <p align="justify" style="font-family:roboto;"> É uma ferramenta para projetos UI com excelentes recursos de Design, Prototipagem, Colaboração, Plug-in de Sistema de Projeto, entre outros. Foi empregado pela nossa equipe para realização da metodologia Product Backlog Building (PBB) e criação das Wireframes.</p></li>
          
  <li><a href="https://vempracasa.atlassian.net/">Jira</a>:
  <p align="justify" style="font-family:roboto;"> Ferramenta do método Scrum utilizada para distribuição das atividades do grupo e priorização das demandas. Possibilitando realizar o planejamento das sprints, sendo capaz de registrar o progresso da equipe e do projeto, facilitando o desenvolvimento e acompanhamento da realização de tarefas.</p></li>
    
  <li><a href="https://www.python.org/">Python</a>:
  <p align="justify" style="font-family:roboto;"> É uma linguagem de programação de alto nível, interpretada de script, imperativa, orientada a objetos, funcional, de tipagem dinâmica e forte. Foi utilizada para codificação de scripts de ETL (Extract, Transform, Load) do sistema, realizando a carga dos dados para o MongoDB e SQL Server.</p></li>
    
  <li><a href="https://www.mongodb.com/">MongoDB</a>:
  <p align="justify" style="font-family:roboto;"> É um software de banco de dados NoSQL orientado a documentos, de código aberto e schema free. Foi utilizado para armazenamento das informações oferecidas pelo cliente, além do tratamento dos dados usando a ferramenta Aggregation Framework.</p></li>
  </ul>
 
  
  <h2 style="font-family:roboto;"> Contribuições Individuais :dart:</h2>
  
   <h3> Atribuições como Desenvolvedor Back-end</h3>
  <p align="justify" style="font-family:roboto;"> Como Desenvolvedor Back-End, as atribuições foram relacionadas com a elaboração de Scripts de ETL (Extract, transform, load), tendo em vista as regras de negócio propostas pelo cliente. Foram criados Scripts Python que extraem, transformam e carregam os dados passados pelo cliente, de arquivos ".csv" para o MongoDB e SQL Server. Tratando as inconsistências e padronizando os dados para tratamentos que serão realizados pela Aggregation Framework, uma ferramenta do MongoDB que permite transformação de dados e resultados, por meio da construção de um "pipeline" para realizar operações analíticas.</p>
    <p align="justify" style="font-family:roboto;"> Além disso, o desenvolvimento foi realizado seguindo a Lei Geral de Proteção de Dados (LGPD), cumprindo os protocolos e cuidados para que os dados pessoais processados pela equipe estivessem com a melhor proteção disponível. Com o uso da ferramenta Veracrypt, utilizada nas máquinas que tiveram o acesso aos arquivos enviados pelo cliente, com objetivo de criar um disco criptografado e com acesso restrito para armazenamento dos dados recebidos. Todas as bases de dados que processavam as informações tiveram restrição de acesso por usuários específicos, ou seja, o usuário comum do sistema não tem permissão de visualizar informações não pertinentes a ele.</p>
  <p align="justify" style="font-family:roboto;"> Com finalidade de obter uma rastreabilidade dos dados durante todos os processos do sistema, participei da elaboração de Logs nos scripts de ETL. Logs são informações de histórico dos registro, como por exemplo: onde as informações trafegaram no sistema, em qual data essa operação ocorreu, qual tipo de operação foi processada e se houve algum erro. Esse recurso é gravado no banco de dados MongoDB e em arquivo de extenção ".log". </p>
    <p align="justify" style="font-family:roboto;"> Ademais, colaborei com a configuração dos ambientes de banco de dados, o deploy da base de dados no MongoDB foi realizada pelo <a href="https://www.mongodb.com/atlas/database">MongoDB Atlas</a>. Já para o SQL Server, foi criado um <a href="https://azure.microsoft.com/pt-br/products/azure-sql/database/#overview">Banco de Dados SQL Azure</a> em nuvem.</p>

  <h3> Atribuições como Scrum Master</h3>
  <p align="justify" style="font-family:roboto;"> As atribuições como Scrum Master da equipe foram pertinentes a realizar um bom planejamento e organização das ações do grupo no decorrer das Sprints. No início do projeto, foi realizada uma reunião para definir nosso principal meio de comunicação e a ferramenta para monitoramento de tarefas, assim decidimos utilizar, respectivamente, o Discord e o Jira. Como Master da equipe, fiquei responsável por acompanhar e analisar o progresso do grupo nesses softwares, de modo a observar se todos os integrantes estavam participando das reuniões semanais e se apresentavam alguma dificuldade com a evolução das tarefas, logo atuando da melhor maneira de acordo com a situação.</p>
  <p align="justify" style="font-family:roboto;"> Após a apresentação do problema por parte do cliente, utilizou-se a metodologia Product Backlog Building (<a href="https://www.caroli.org/livro/pbb/">AGUIAR; CAROLI, 2021</a>) para a elaboração de um Backlog conciso com as necessidades do cliente. Obtendo como resultado final desse processo as User Stories que compõe o Product Backlog e a descrição da experiência do usuário com o produto, além de promover um ótimo entendimento das regras de negócio e os primeiros questionamentos para o cliente. Com esse alinhamento inicial finalizado, as User Stories foram divididas entre as 4 Sprints do projeto, dessa forma tive a função de quebrar essas histórias em tarefas menores e mais objetivas, para um melhor desenvolvimento do que foi planejado, e também delegar essas tasks entre os integrantes da equipe.</p>
  <details>
  <summary>Clique aqui para visualizar a organização de uma Sprint no Jira</summary>
  <br>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/API6Sem-Jira1.png" width="1000px;" alt=""/>
   <img style="border-radius: 50%;" src="https://github.com/GabrielSG20/Portfolio/blob/main/images/API6Sem-Jira2.png" width="1000px;" alt=""/>
  </details>
  
   <h2 style="font-family:roboto;"> Funcionamento :bulb:</h2>

   <div align="center">
     <img src="https://github.com/GabrielSG20/Portfolio/blob/resume/assets/img/6SemSolucao.png" style="max-rate: 730px;"></img>    
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
      <td>★★★★★★★★☆☆</td>
    </tr>
    <tr>
      <td>Python</td>
      <td>★★★★★★★★☆☆</td>
    </tr>
    <tr>
      <td>MongoDB</td>
      <td>★★★★★★★★☆☆</td>
    </tr>
    <tr>
      <td>Microsoft SQL Server</td>
      <td>★★★★★★★★☆☆</td>
    </tr>
    <tr>
      <td>Cloud</td>
      <td>★★★★★★★☆☆☆</td>
    </tr>
     <tr>
      <td>GIT</td>
      <td>★★★★★★★★★☆</td>
    </tr>
  </table>
  
  <h3 align="center">Soft Skills</h3>
      <table align="center">
    <tr>
      <th width="300px">Habilidade</th>
      <th width="300px">Descrição</th>
    </tr>
    <tr>
      <td>Responsabilidade</td>
      <td>Assumi novamente o cargo de Scrum Master.</td>
    </tr>
    <tr>
      <td>Comunicação</td>
      <td>Precisei me comunicar com a equipe para saber a evolução das tarefas na SPRINT.</td>
    </tr>
    <tr>
      <td>Organização</td>
      <td>Precisei organizar a documentação e código no GitHub.</td>
    </tr>
    <tr>
      <td>Planejamento</td>
      <td>Precisei quebrar as tarefas das SPRINT's, colocando datas limites.</td>
    </tr>
    <tr>
      <td>Visão de Negócio</td>
      <td>Compreendi melhor os problemas e expectativas do cliente, utilizando a metodologia Product Backlog Building.</td>
    </tr>
  </table>
  
---

 <h2 align="center"> Navegação Projetos :link:</h2>
 
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/GabrielSG20/Portfolio/blob/main/API_1.md"> 1º Semestre: Assistente Virtual para Idosos - O app que facilita o uso de smartphones para usuários da terceira idade</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/GabrielSG20/Portfolio/blob/main/API_2.md"> 2º Semestre: Trinity - Cadastro e análise de contas com mais simplicidade</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/GabrielSG20/Portfolio/blob/main/API_3.md"> 3° Semestre: AirPLAN - O software que otimiza a criação e controle de documentos de aeronaves</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/GabrielSG20/Portfolio/blob/main/API_4.md"> 4° Semestre: #VEMPRACASA - Uma plataforma de gerenciamento de eventos</a></li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/GabrielSG20/Portfolio/blob/main/API_5.md"> 5º Semestre: Data Rangers - Ferramenta de análise de dados para prospecção de novos clientes</a></li></p>
   <p align="justify" style="font-family:roboto;"><li>6º Semestre: D-end - Processamento e análise de dados para tratamento de inconsistências</li></p>
   <p align="justify" style="font-family:roboto;"><li><a href="https://github.com/GabrielSG20/Portfolio/blob/main/README.md"> Voltar para página inicial</a></li></p>

</body>
</html>
