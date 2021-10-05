# Repositorio do desafio GitHub
Desafio Sobre Projeto de GitHub

### :computer: O que é GitHub
Git é uma ferramenta de controle de versão, desenvolvida por nada menos que Linus Torvalds. Nessa primeira parte vou ensinar como instalar, e configurar para começar a usá-lo com o github (Criar um repositório e enviar projetos no seu portifolio). E também como você pode versionar seus projetos para trabalhar melhor.

### :computer: O que é um controle de versão? 
é um sistema que armazena as alterações realizadas em um arquivo ou vários arquivos durante o tempo, de modo que você consiga resgatar versões específicas.

<img src="https://user-images.githubusercontent.com/77301626/136073245-97c66d95-c22c-4306-9b65-5742cbadaeae.png">

Obs: Caso Você não tenha instalado!
Site Oficial: https://git-scm.com/downloads

----
* Nesse projeto vamos utilizar o github que é um serviço web que tem várias funcionalidades extras para o git. É como se fosse uma rede social de desenvolvedores, onde você pode ver o código de outros desenvolvedores, clonar projetos na sua máquina, contribuir com a comunidade com os projetos open-source. Então se você não se cadastrou ainda, não perca tempo e faça o cadastro.

* Depois de feito o cadastro vamos criar o nosso primeiro repositório que é local onde vai ser armazenado o código do nosso projeto, basta ir em Repositories no seu perfil do github e clicar em New.

<img src="https://user-images.githubusercontent.com/77301626/136073566-eb82ef83-50b0-4ae4-b2eb-c804061f9f5c.png">

* No Repository name, você vai colocar o nome do repositório. Você pode adicionar uma descrição se quiser. E inicializar com o arquivo README.md que é o arquivo onde você pode colocar as instruções de como instalar seu projeto.

<img src="https://user-images.githubusercontent.com/77301626/136074064-89126c3a-d8ad-41d0-9eeb-197623f91d71.png">

* Logo após a criação do repositório é possível ver alguns comandos que vão ser utilizados no decorrer do post.

# Configurações iniciais do git

Para utilizar o git e enviar seus arquivos para o github, é preciso configurar em sua máquina seu usuário e email do github.

$ git config --global user.name "Seu Nome"

$ git config --global user.email Seu Email

*Se quiser Conferir digita: $ git config --list

---


# Enviando Projeto

* Entre na pasta do projeto.
$ cd project/

* inicialize o git
$ git init

Com esse comando, o git vai criar uma pasta oculta com o nome ./git para ter a estrutura que vai ser utilizada para controlar seus arquivos, salvar as branchs, salvar o histórico, etc.
* é possível saber o status dos arquivos na máquina. Vamos usar o git status.

<img src="">

Todos os arquivos estão em vermelho, isso quer dizer que nenhum arquivo está sendo monitorado. Para monitorar arquivos basta digitar
