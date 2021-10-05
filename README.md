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
* Nesse projeto vamos utilizar o github que é um serviço web que tem várias funcionalidades extras para o git. É como se fosse uma rede social de desenvolvedores, onde você pode ver o código de outros desenvolvedores, clonar projetos na sua máquina, contribuir com a comunidade com os projetos open-source.

* Depois de feito o cadastro vamos criar o nosso primeiro repositório que é local onde vai ser armazenado o código do nosso projeto, basta ir em Repositories no seu perfil do github e clicar em New.

<img src="https://user-images.githubusercontent.com/77301626/136073566-eb82ef83-50b0-4ae4-b2eb-c804061f9f5c.png">

* No Repository name, você vai colocar o nome do repositório. Você pode adicionar uma descrição se quiser. E inicializar com o arquivo README.md que é o arquivo onde você pode colocar as instruções de como instalar seu projeto.

<img src="https://user-images.githubusercontent.com/77301626/136074064-89126c3a-d8ad-41d0-9eeb-197623f91d71.png">

* Logo após a criação do repositório é possível ver alguns comandos que vão ser utilizados no decorrer do post.

# Configurações iniciais do git

Para utilizar o git e enviar seus arquivos para o github, é preciso configurar em sua máquina seu usuário e email do github.

$ git config --global user.name "Seu Nome"

$ git config --global user.email Seu Email

* Se quiser Conferir digita: $ git config --list

---


# Enviando Projeto

* Entre na pasta do projeto.
$ cd project/

* inicialize o git
$ git init

Com esse comando, o git vai criar uma pasta oculta com o nome ./git para ter a estrutura que vai ser utilizada para controlar seus arquivos, salvar as branchs, salvar o histórico, etc.
* é possível saber o status dos arquivos na máquina. Vamos usar o git status.

<img src="https://user-images.githubusercontent.com/77301626/136078506-6d001870-6026-4436-9454-073d5b800abd.png">

Todos os arquivos estão em vermelho, isso quer dizer que nenhum arquivo está sendo monitorado. Para monitorar arquivos basta digitar

#### Adiciona apenas um arquivo
$ git add <file>.  Adiciona uma pasta com seu conteúdo
$ git add <directory> Adiciona todas as modificações feitas
$ git add -A or git add .

Nesse caso como não tem nada no nosso repositório, vamos adicionar toda a estrutura inicial do projeto, então vamos utilizar o git add .
Depois com o comando git status é possível ver que todos os arquivos foram adicionados com sucesso.
  
---
# Git commit

O commit serve para você adicionar uma descrição das modificações feitas nos arquivos, nesse caso como só vou adicionar os arquivos no master do repositório, só adicionei “First commit”, mas em outras alterações você pode adicionar especificamente o que aquele commit pode fazer, por exemplo: “Add user page”.
  
<img src="https://user-images.githubusercontent.com/77301626/136079737-4b31affd-1dbf-4bc9-8c77-ca57aee32bb8.png">
 
Se você digitar git status, agora verá que todos os arquivos foram commitados. E não tem nenhuma alteração no diretório de trabalho
  
<img src="https://user-images.githubusercontent.com/77301626/136079842-c141390b-808a-43be-abbf-d21f186b5f20.png">

Antes de enviar as alterações precisamos especificar o link do repositório remoto. Você consegue o link indo em seu repositório criado, na aba Code. Nesse tutorial eu vou utilizar o protocolo SSH para não precisar ficar digitando usuário e senha em toda conexão que ele fizer com o github.

Se for utilizar SSH é preciso fazer a configuração, eu traduzi um tutorial do help do github, afirmo que é melhor você usar SSH para agilizar o trabalho. Mas você também pode utilizar o HTTPS fica a seu critério.

Copie o link.

<img src="https://user-images.githubusercontent.com/77301626/136080140-bb026267-a7ef-4cc0-af1b-c896d5de9c7b.png">
  
E rode o comando:

$ git remote add origin Seu_link
  
<img src="https://user-images.githubusercontent.com/77301626/136080288-912ed12a-bb0e-4010-a041-230c7daa8fc8.png">
  
Para verificar se deu certo:

$ git remote -v
# Isso vai listar o link dos seus repositórios remotos

Git push (Enviar atualizações)

Finalmente vamos enviar as alterações para o github. O comando basicamente é:

$ git push -u origin <branch>.
# Nesse caso como é nossa estrutura inicial vamos enviar para o master.

Colocando o -u junto com o push ele faz o set-upstream que seria fazer a referência do repositório remoto com a devida branch.
  
<img src="https://user-images.githubusercontent.com/77301626/136080491-a72c8b76-8378-49b0-aa2f-10f6a3415686.png">
  
Depois de aperte F5 na pagina do repositorio e vuala!
  
<img src="https://user-images.githubusercontent.com/77301626/136080636-365ffe79-6d2f-4416-a9dd-8c5f93f2d8b2.png">
