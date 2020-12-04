
## GIT COMANDOS

## Criando repositorio
git init

## Verificando as mudancas
git status

## Adicionando atualizaçoes
git add .

## Confirmando atualiacao
git commit -m "Atualizando Repositorio"

## Enviando para master
git push -u  origin master

## Avaliando log
git log


## FLUXO DE DESENVOLVIMENTO
<1>
git checkout -b dev  
>criando uma branch dev e mudando

git branch dev 
>cria mas nao muda

git branch 
>identificaro a branch selecionada

*dev
 master

<2>
@Realize as modificações (trabalhe)

<3>
@Persistir os dados na branch DEV
gitt add && git commit -m "Segundo commit" 
> adicionando e commitando na dev

<4>
@Fazendo uma nova branch para equipe
git checkout -b feature-1 dev 
> so vai consegui ir para outra branch se nao tiver pendencia de commit na branch atual (Already up-to-date.)

> criando uma branch apartir das informacoes da dev

  dev
 *feature-1
  master 


<5>
@Persistindo dados na branch FEATURE
## Info

<6 - mergo e nao push/pull-requeste>
@Merge manual que nao tenha um pull requeste
git checkout dev 
> mudando para dev 

git merge --no-ff feature-1 
>--no ff => Git fast forwards junta um commit novo forcando

git commit -m "atualizando"

<7>
@Criando outra release da dev
git checkout -b feature2
git branch 
  dev
  feature-1
>nova release criada agora bastar trabalhar

*feature2
  master

git add . && git commit -m "Feature 2"
>Persistindo



<8>
@Push (externo - github)
git remote add origin https://github.com/pabloverly/Git_Command.git
>adicionando conexao remota

git remote -v
>verificando o link 

git push origin master
>enviando a master local para master remoto





# plugin
git blame para vscode 
>Mostra o autor dos commits

