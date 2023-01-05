# 10 Comandos do Git que todo desenvolvedor deveria conhecer

<!-- <img src = "https://upload.wikimedia.org/wikipedia/commons/thumb/e/e0/Git-logo.svg/640px-Git-logo.svg.png"> -->

O Git é uma parte importante da programação no dia a dia.
Como existem muitos comandos que você pode utilizar, dominar o Git por completo leva tempo.

## 1 Git status

O comando git status nos dá todas as informações necessárias sobre a branch atual.

`git status`

<img src ='https://cdn1.gnarususercontent.com.br/1/796210/6f40f47b-8443-4be9-8435-21ba33853d2a.png'>

Git status nos dá informações sobre a branch e os arquivos
<ul>
    <li>Se os arquivos estão em fase de stage, fora dessa fase ou se não estão sendo rastreados</li>
    <li>Se arquivos foram criados, modificados ou excluídos</li>
    <li>Se a branch em que estamos no momento está atualizada</li>
    <li>Se precisamos fazer o commit, push ou pull de algo</li>
</ul>

## 2 Git add

O comando git add adiciona uma alteração no diretório ativo à área de staging

### Para adicionar um único arquivo:

`git add <arquivo>`

### Para adicionar tudo ao mesmo tempo::

`git add .`

<img src = 'https://lh3.googleusercontent.com/09H2vyZqfHKuW6F0O3Omy5XwoqBuQh7P_74Pdn5HnYCTwFiOXtTf7S8BjBlyVpqicT1MHWkSoRgSwCxvpdPhBCj2kPZk-6_z9Alq0cclrO5UbZBauSx7--8215IfnR5k5RidY67K'>

Os arquivos em verde agora estão em fase de stage com o git add

## 3 Git commit

Git commit é como definir um ponto de verificação no processo de desenvolvimento. Você pode voltar a esse ponto mais tarde, se necessário.

`git commit -m "mensagem do commit"`



## 4 Git push

Git push faz o upload dos seus commits no repositório remoto.

`git push <repositório-remoto> <nome-da-branch>`

Se a sua branch foi recém-criada, também é preciso fazer o upload da branch com o seguinte comando:

`git push -u origin <nome-da-branch>`

## 5 Git branch

O comando git branch permite criar, listar, renomear e excluir ramificações.

<img src ='https://lh5.googleusercontent.com/ByJxAPDtlT6I3uHFZeoXRiYwyrVkdIY6Iho8chNGp4DL9Ke8snH9SKCYs10G0bWf-xc_DMgcRIpvrQw0LbQ809tdpi6SBx7lyQ2W6ZRI5EhUFO4jkVLPw3SuAxoGik97qWYg_Kmm'>

### Como criar uma branch:
`git branch <nome-da-branch>`

Para fazer o  push  da nova branch para o repositório remoto, você precisa usar o comando a seguir:

`git push -u <local-remoto> <nome-da-branch>`
<br>

### Como ver as branches:
`git branch ou git branch --list`

### Como trabalhar apartir da branch criada:
`git checkout nomeDaBranch`

### Como emviar sua branch ao GItHub:
`git push -u origin nome_branch`

### Como excluir uma branch:
`git branch -d <nome-da-branch>`

### Como expluir uma branch remota:
`git push origin --delete nome_branch`

## 6 Git checkout

Para trabalhar em uma branch, primeiro, é preciso "entrar" nela. Usamos git checkout, na maioria dos casos, para trocar de uma branch para outra. Também podemos usar o comando para fazer o checkout de arquivos e commits.

Passos que você precisa seguir para trocar de branch com sucesso:


- As alterações em sua branch atual devem estar em um commit ou em um stash antes de você fazer a troca
- A branch na qual você quer fazer o checkout deve existir no seu espaço de trabalho local


## 7 Git pull

O comando git pull é usado para buscar e baixar conteúdo de repositórios remotos e fazer a atualização imediata ao repositório local para que os conteúdos sejam iguais.

`git pull <repositório-remoto>`


## 8 Git log

Com o comando git log, você pode visualizar o que vem sendo feito em uma determinada branch ou avaliar as alterações de um arquivo em especial.

`git log --oneline`

<img src = 'https://www.cloudsavvyit.com/p/uploads/2021/08/963731e4.png?trim=1,1&bg-color=000&pad=1,1'> 

Em amarelo temos o código hash ao lado do commit.

## 9 Git Clone
O git clone, basicamente, faz uma cópia idêntica da versão mais recente de um projeto em um repositório e a salva em seu computador.

`git clone <https://link-com-o-nome-do-repositório>`

## 10 Git revert

Umas das maneiras de alterações em nosso espaço de trabalho local ou remotamente. Uma maneira segura de desfazer nossos commits é usando git revert

`git revert <name hash>`

Precisamos apenas especificar o código hash ao lado do commit que desejamos desfazer:

### Para  reverter especificamente o último commit podemos usar também:
`git revert HEAD`
