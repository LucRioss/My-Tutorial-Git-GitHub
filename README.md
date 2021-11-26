# My-Tutorial-Git-GitHub
Tutorial  básico de Git e GitHub feito para ser claro e objetivo 


`git init` para inicializar o repositório.

`git add` para enviar os arquivos para área de staging

`git commit -m “nome do commit”` o commit para que vem do SQL tem a mesma função tornar permanente a alteração, mais para o Git e atualizar o que está na área de staging esse commit ficar marcado a alteração do que foi realizada

`git branch -M “main”` esse comando tem a função de atualizar o nome da branch que está, a branch nada mais é que uma ramificação do estado atual do programa onde, se pode fazer alteração sem mexer na branch principal mantendo assim a “estabilidade” do código e podendo voltar para branch anteriores são a algum tipo de alteração a ser corrigida.

`git remote add origin “link do repositório”` onde esse comando tem a função de fazer a conexão como o repositório através do link e logo após a verificação a conexão está feita (origin e nome utilizado para referenciar o repositório)

`git push -u origin main` mesmo feito o commit os arquivos não são colocados no repositório sendo necessário empurrar(Caso os arquivos não apareça de imediato atualizar a pagina).

`git add .` a função desse comando e enviar todas as alterações feita para a area de staging, lembrando que após utilizar esse comando realizar o commit e push (`git commit -m "alteração"` `git push origin main`) sem o -u

## Criação de Branch

#### Branch Ramificação, em controle de versão e gerenciamento de configuração de software, é a duplicação de um objeto sob controle de versão. Cada objeto pode, a partir daí, ser modificado separadamente e em paralelo para que os objetos se tornem diferentes.(Wikipedia)

`git checkout -b "nome-da-branch"` a utilização desse comando cria a brach o ‘checkout’ já traz a branch junto, onde é mostrado o lado do nome do repositório, assim se cria os arquivos que vão entrar na branch, assim para enviar os arquivos realizar os mesmo comandos como se estive na branch principal (`git add .` `git commit -m "nome do commit"` `git push origin nome-da-branch`).

`git checkout “nome-da-branch”` caso precise mudar de branch para alterar é só utilizar o git checkout + o nome da branch desejada

`git merge nome-da-branch` caso queira fazer a junção das duas branch por exemplo branch1 e branch2, terá que ir na branch anterior (branch1) e digitar o comando git merge branch2 como por exemplo assim as duas estarão na branch principal e finalizar git push origin nome-da-branch-principal
