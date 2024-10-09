# DIO | RESUMOS Git e GitHub

Repositório para armazenar resumos sobre Git e GitHub do curso Versionamento de Código com Git e GitHub da [Digital Innovation One](https://www.dio.me/).

## Documentação
- [Documentação Git](https://git-scm.com/doc)
- [Documentação GitHub]()

## Resumo das Aulas

| Aulas | Resumos |
|-------|---------|
|Gravando Alterações do Repositório Local | [Resumos] () |

```
git init
git remote add origin (URL do repositório)
git status
touch README.md
git add README.md
git commit -m"descrição do commit"
touch resumos/resumo-aula1.md
echo resumos/ > .gitignore

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
```
## Referências
- [Digital Innovation One] ()