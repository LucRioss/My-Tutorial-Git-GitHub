Git e GitHub

●	git init para inicializar o repositório.

●	git add para enviar os arquivos para área de staging (uma área de espera para ser upado para o repositório)

●	git commit -m “nome do commit” o commit para que vem do SQL tem a mesma função tornar permanente a alteração, mais para o Git e atualizar o que está na área de staging esse commit ficar marcado a alteração do que foi realizada

●	git branch -M “main” esse comando tem a função de atualizar o nome da branch que está, a branch nada mais é que uma ramificação do estado atual do programa onde, se pode fazer alteração sem mexer na branch principal mantendo assim a “estabilidade” do código e podendo voltar para branch anteriores são a algum tipo de alteração a ser corrigida.

A partir disso, é necessário a criação de uma conta no GitHub e ir em “novo repositório” colocar nome da pasta e a descrição (sendo opcional).	Após isso é gerado um link para a pasta que iremos usar

●	git remote add origin “link do repositório” onde esse comando tem a função de fazer a conexão como o repositório através do link e logo após a verificação a conexão está feita (origin e nome utilizado para referenciar o repositório)
●	git push -u origin main mesmo feito o commit os arquivos não são colocados no repositório sendo necessário empurrar.

Assim é só atualizar a página e já é possível visualizar os arquivos

Alteração de arquivos ou adicionar novos arquivos

●	git add . a função desse comando enviar todas as alterações feita para a staging, lembra que após realizar o commit e push (git commit -m "alteração" -  git push origin main) sem o menos -u


Branch
	Ramificação, em controle de versão e gerenciamento de configuração de software, é a duplicação de um objeto sob controle de versão. Cada objeto pode, a partir daí, ser modificado separadamente e em paralelo para que os objetos se tornem diferentes.(Wikipedia)

●	git checkout -b "nome-da-branch" a utilização desse comando cria a brach o ‘checkout’ já traz a branch junto, onde é mostrado o lado do nome do repositório, assim se cria os arquivos que vão entrar na branch, assim para enviar os arquivos realizar os mesmo comandos como se estive na branch principal (git add ., git commit -m "nome do commit", git push origin nome-da-branch).

●	git checkout “nome-da-branch” caso precise mudar de branch para alterar é só utilizar o git checkout + o nome da branch desejada

●	git merge nome-da-branch caso queira fazer a junção das duas branch por exemplo branch1 e branch2, terá que ir na branch anterior (branch1) e digitar o comando git merge branch2 como por exemplo assim as duas estarão na branch principal e finalizar git push origin nome-da-branch-principal
