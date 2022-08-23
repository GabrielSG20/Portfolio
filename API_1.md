<html>
<body>
 <h1 align="center"> API 1º Semestre - 01/2020</h1>
  
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

</body>
</html>
