# DIO | RESUMOS Git e GitHub

Repositório para armazenar resumos sobre Git e GitHub do curso Versionamento de Código com Git e GitHub da [Digital Innovation One](https://www.dio.me/).

## Documentação
- [Documentação Git](https://git-scm.com/doc)
- [Documentação GitHub]()

## Resumo das Aulas

| Aulas | Resumos |
|-------|---------|
|Gravando Alterações do Repositório Local | [Resumos] () |

## Comandos Git
```
git config --global user.name "Nome"
git config --global user.email "email"
git config --global init.defaultBranch nomeDaBranch

git init
git remote add origin (URL do repositório)
git status
touch README.md
git add README.md
git commit -m"descrição do commit"
touch resumos/resumo-aula1.md
echo resumos/ > .gitignore
git log  //mostra todos os commits realizados

rm -rf .git  //vai excluir o versionamento, caso tenha dado init na pasta errada
git restore README.md  //Vai voltar a modificação mais recente, caso queira deletar as alterações feitas
git commit --amend -m"nova descrição para o commit"  //Altera a mensagem do último commit
git reset --soft (aqui vai o código do commit) //pega todos os commits anteriores ao indicado aqui e levam suas alterações feitas para a área de preparação novamente e os commits deixam de existir
git reset --mixed (aqui vai o código do commit)  //Diferente do soft que vimos acima, no mixed os arquivos ainda precisam ser adicionados na área de preparação, ou seja, ainda não são reconhecidos ao contrário do soft
git reset --hard (aqui vao o código do commit)  //Aqui ele desfaz os arquivos dos commits, ele exclue todos eles
git reflog  //Vai mostrar todos os commits realizados
git reset (nome do arquivo)  //Vai retirar esse arquivo da área de preparação
git restore --staged (nome do arquivo)  //Vai remover os arquivos que haviam sido commitados

git push -u origin main  //o "push" é o responsável por enviar as alterações do repositório local para o remoto
git pull  //o "pull" vai buscar as alterações feitas no repositório remoto e mesclar com o nosso repositório local

git checkout -b nomeDaNovaBranch  // Cria uma nova branch e altera a atual em que você está para a nova
git checkout nomeDaBranch  // Altera a branch em que você está para a indicada no comando
git branch -v  // Mostra o último commit de todas as branchs existentes
git branch  // Lista todas as branchs
git merge  // Usamos para poder mesclar branchs, por exemplo uma alteração feita na branch "teste" que não tem na "main", então fazemos um merge dentro da branch "main" apontando para a "teste"
git branch -d nomeDaBranch  //Exclui uma branch

git fetch origin main  //Comando útil para quando você apenas quer apenas baixar o conteúdo da branch remota sem mesclar com a branch local
git clone (URL do repositório) --branch nomeDaBranch --single-branch  //Serve para você poder clonar apenas uma branch específica
git stash  //Esse comando arquiva uma modificação, é útil para situações quando você não quer que uma alteração específica suba para a main quando você for darum merge por exemplo
git stash list  //Vai listar todas as alterações arquivadas
git stash apply //É para quando você quer trazer de volta as modificações que foram arquivadas e também deseja manter essas mesmas modificações na lista de arquivados
git stash pop //Esse comando é igual ao apply, a diferença é que ele exclui as alterações das listas de arquivadas
```
## Referências
- [Digital Innovation One] ()