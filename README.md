# aula_git2

#### Arquivos de exemplo para utilização basica/incial do Git (foco na criação de branch's).

## Iniciando...

##### "Configurando o git local"
* [criar posteriormente] <!-- //TODOrefatorar ordenação dos itens -->

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

* `git branch` indica a(s) branch(s) existente(s) no repo
* `git branch novabranch2` cria uma "novabranch2" mas não a acessa
* `git checkout -b novabranch` 
Cria e entra automaticamente dentro desta nova branch sendo retornado no terminal: **Switched to a new branch 'novabranch'**<br>

* `git status` indicara o status do repo atual<br>
* Adicione os arquivos modificados como antes: `git add .`<br>
* `git add arquivo.txt` adiciona exclusivamente um unico arquivo<br>
* `git reset head arquivo.txt`<br> "remove" o este arquivo
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


## Criando um Pull Request 
* [em produção/breve]

## Removendo uma Branch (Local)

`git branch -d novabranch2` remove a branch "novabranch2"

**Obs.:** 
*A opção __-d__ (–delete) removerá o branch local se você já a tiver enviado e mesclado às ramificações remotas.*

*A opção __-D__ (–delete –force) removerá o branch local, independentemente de você ter enviado e mesclado com as ramificações remotas.*

## Removendo uma Branch (Remoto)

`git push origin --delete novabranch2`

## Atualizando repositorio local, com dados do remoto
* `git fetch origin` baixa atualizações, em cache
* `git pull` aplica atualizações localmente

<hr>

#### Links do youtube: 
* <https://www.youtube.com/watch?v=NR9jc5ODvuM&list=PL8iIphQOyG-BZ2y75BepyrFz-wqOIOHvf>
* <https://www.youtube.com/watch?v=dSUT0Y7suPI>


##### Referencia sobre markdown:
<https://docs.pipz.com/central-de-ajuda/learning-center/guia-basico-de-markdown#open>

##### Referencias sobre Git:
<https://receitasdecodigo.com.br/devops/git-remover-um-branch-local-ou-remoto>