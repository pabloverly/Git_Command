
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

> criando uma branch apartir das informacoes da dev

  dev
 *feature-1
  master 


<5>
@Persistindo dados na branch FEATURE
## Info

<6>
@Merge manual que nao tenha um pull requeste
git checkout dev 
> mudando para dev 

<6>
git merge --no-ff feature-1 
>--no ff => Git fast forwards junta um commit novo forcando



