# aula_git2

#### Arquivos de exemplo para utilização basica/incial do Git (foco na criação de branch's).

## Iniciando...

##### Procedimentos locais
* Criar a pasta do repositorio local, ex.: `aula_git2`
* Entrar na pasta: `cd aula_git2`
* Criar os arquivos inciais do projeto
* Iniciar o repo: `git init`
* adicionar (tod)os arquivos a verificação do git: `git add .`
* Efetuar o primeiro commit: `git commit -m "primeiro commit"`<br>
*isso retorna informação que os arquivos foram adicionados*

##### Procedimentos remotos
* criar o repositorio na pagina do git*(hub, lab, etc)*
* copiar link do repositorio e executar dentro do projeto:
`git remote add origin https://github.com/thanakin/aula_git2.git`
* enviar os arquivos "commitados" ao repositorio remoto: `git push`
* inserir **usuario** e **senha** do git

<hr>

## Criando uma nova Branch

* No terminal: `git checkout -b novabranch`<br>
*Apos este comando, ja estara automaticamente dentro desta nova branch sendo retornado no terminal: **Switched to a new branch 'novabranch'***<br>
* `git status` indicara o status do repo atual<br>
* Adicione os arquivos modificados como antes: `git add .`<br>
* Realize o commit das mudanças: `git commit -m "testando nova branch"`<br>
* Os arquivos agora podem ser enviados ao repo remoto:<br>
`git push origin novabranch`<br>
*retornara o status deste novo envio*<br>
* Para "voltar" a master: `git checkout master`
*no teste local, a master estava nomeada como "main"*
* Unificando as mudanças da novabranch para a master:
`git merge novabranch`<br>
* Na sequencia, adiciona os arquivos modificados:
`git add .`
* Fazer um commit pertinente:
`git commit -m "fazendo merge da novabranch com master"`
* Para enviar tudo ao repo remoto:
`git push`


<hr>

#### Link da playlist: 
<https://www.youtube.com/watch?v=NR9jc5ODvuM&list=PL8iIphQOyG-BZ2y75BepyrFz-wqOIOHvf>


##### Referencia sobre markdown:
<https://docs.pipz.com/central-de-ajuda/learning-center/guia-basico-de-markdown#open>