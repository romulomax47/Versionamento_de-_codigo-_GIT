## 10 comandos do Git que todo desenvolvedor deveria conhecer

<img src = "https://upload.wikimedia.org/wikipedia/commons/thumb/e/e0/Git-logo.svg/640px-Git-logo.svg.png">

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

## 3. Git commit

Git commit é como definir um ponto de verificação no processo de desenvolvimento. Você pode voltar a esse ponto mais tarde, se necessário.

`git commit -m "mensagem do commit"`

## 4. Git push

Git push faz o upload dos seus commits no repositório remoto.

`git push <repositório-remoto> <nome-da-branch>`

Se a sua branch foi recém-criada, também é preciso fazer o upload da branch com o seguinte comando:

`git push -u origin <nome-da-branch>`


