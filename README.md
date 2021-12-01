# My-Tutorial-Git-GitHub



`git init` Serve para inicializar o repositório Git (lembrado que tem que estar dentro do diretório dos arquivos desejados, para esse facilitar caminho é só clicar com o botão direito do mouse dentro do diretório desejado e clicar com o botão esquerdo na janela seguinte em ` “Git Bash Here” `. 

<image1>
<img src="https://imgur.com/W4I5bYL.png" height="450" width="600">
Bash do Git:
<image2>
<img src="https://i.imgur.com/nDmhyHY.png" height="400" width="500">
 

`git add nomedoarquivo.formato` Enviar os arquivos para área de staging do Git

`git commit -m “nome do commit”` O commit tem a função de tornar algo permanente, o mesmo acontece com Git as alterações que add encaminhou para a área de staging o commit envia para o repository, mesmo assim não é suficiente para aparecer no github outros comandos são necessários para isso ser realizado.
  
Agora o próximo passo é dentro do GitHub, após criar a conta ou fazer o login, clicar no ícone do seu perfil e ir em seus repositórios como na imagem a seguir.

<image3>
<img src="https://i.imgur.com/RE82hRI.png">
 
Após isso, uma janela vai ser carregada, para criar um repositório é só clicar no botão new que vai estar em foco na cor verde.

<image4>
<img src="https://i.imgur.com/3Cov5U3.png">
 
 Depois disso outra janela vai ser carrega onde é possível colocar o nome do repositório, descrição e a opção se vai público ou privado, depois é só clicar no botão "Create Repository" para criar, as caixas de opções:  o `readme` (leia me) tem a função de ser a porta de entrada onde pode conter a descrição do código, explicação das funções, etc, nesse caso está servindo para esse tutorial. 	O `.gitgnore` serve para dizer ao Git quais arquivos ignorar já `Choose a license` ele é o contrato de licença para o repositório do GitHub, ele diz aos outros usuários o que podem ou não fazer com os arquivos do repositório, para mais informações e só clicar em `Learn more`
  
<image5>
<img src="https://i.imgur.com/P1l1FUo.png" height="600" width="600">
  
 Após criar o diretório na próxima tela um link irá ser gerado, no caso podemos ver que é um link padrão onde ele segue o formato:
  
`https://github.com/NOMEDOSEUPERFIL/NOMEDOREPOSITORIO.git`<br>
  
E abaixo do link podemos ver a lista de comandos necessário para enviar os arquivos ao repositório do GitHub agora com o link em mãos voltamos ao bash do git para prosseguir.

<image6>
<img src="https://i.imgur.com/bjDt2xC.png" >

`git remote add origin link-do-repositório` Esse comando tem a função de fazer a conexão como o repositório através do link assim a conexão está feita (origin é nome utilizado para referenciar o ddiretório que está sendo enviado)

`git push -u origin main` Tem a função de empurrar os arquivos do commit para o repositório do GitHub(Caso os arquivos não apareça de imediato atualizar a pagina).

`git add .` A função do Git add + o ponto é de enviar todas as adições feita para a área de staging, lembrando que após utilizar esse comando realizar o commit e push (`git commit -m "adição"`  `git push origin main` sem o "-u" isso poque como pode se observar pela própria tabela que se encontra no livro Pro Git disponibilizado na plataforma di Git ele significa update -página 23).
 
<image7>
<img src="https://i.imgur.com/qIdShhj.png" height="400" width="500">
 
Para acessar fazer download do Livro e tanto do propriamente dito Git, acessar a página oficial do Git.
 
<image8>
<img src="https://i.imgur.com/3MyIt1i.png" height="350" width="900">  
 
## Criação de Branch

####  Branch Ramificação, em controle de versão e gerenciamento de configuração de software, é a duplicação de um objeto sob controle de versão. Cada objeto pode, a partir daí, ser modificado separadamente e em paralelo para que os objetos se tornem diferentes.(Wikipedia)

`git checkout -b "nome-da-branch"` A utilização desse comando cria uma branch, onde é mostrado o lado do nome do repositório o nome da branch assim indicando em qual branch está.    Assim que criado os arquivos para essa branch o processo de enviar e mesmo de como estive na branch principal só alterando o nome para a branch atual (`git add .` `git commit -m "nome do commit"` `git push origin nome-da-branch`) assim é criado uma versão com os arquivos que contêm a adição/alteração mais os arquivos residiam antes.

`git checkout “nome-da-branch” ` Tem a função de mudar de branch assim pode transitar entre várias branch.
  
`git branch -M “main” ` Esse comando tem a função de atualizar o nome da branch em que está.

`git merge nome-da-branch` Caso queira fazer a junção de duas branch, terá que ir à branch anterior a que você irá mesclar e digitar o comando como por exemplo, duas branch a Main e a Update se o bash estiver localizado na Update a junção não acontecerá assim sendo necessário voltar para a branch anterior a Main assim e possível a junção, quando `merge` é feito os arquivos adicionado/alterados no Update será mesclado a branch Main.
  
 ## Alterações no Repositório do GitHub
  
`git pull` Quando uma alteração e feita pelo GitHub ou através de outra máquina ou colaborador o arquivo que está na máquina fica desatualizado, para fazer a atualização é necessário estar no diretório e digitar `git pull` assim toda adição/alteração feita até aquele determinado momento será atualizado levando em conta que arquivos excluídos no repositório do github ele também será excluído do seu diretório.

## Considerações Finais
  
Eu escolhi esse tutorial para ser o meu primeiro repositório para deixar como documento explicado em minhas palavras para mim e para quem achar útil, caso esteja iniciando considere fazer o seu próprio tutorial por mais simples que seja isso ajudar a fixar os comandos e como a plataforma funciona, isso tem me ajudado a entender e criar dúvidas de como realizar determinados procedimentos e buscar sanar eles. 	Bom espero que tenha sido de grande aproveito esse tutorial, agradeço e até mais  =)

 ### Extra 
 
`git checkout <sua-branch> && git pull origin <sua-branch>`
 
`git remote rm origin` Elemina a conexão com o link atual do repositório
 
`git remote set-url origin link-novo` Troca o link do Repositório
 
`git push origin <sua-branch> --force` USAR COM CUIDADO ELE FORÇA A ATUALIZAÇÃO COM O REPOSITORIO ONLINE PODE APAGAR OS ARQUIVOS SE ELES NÃO ESTIVEREM ATUALIZADOS

`git config --global https.proxy`
