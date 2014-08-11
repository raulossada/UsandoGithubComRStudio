
# Criando um GitBook

1) Uma vez que o pacote ``Rgitbook`` esteja instalado e carregado, para criar um novo livro, basta usar a função: **newGitbook()**, passando como parâmetro o nome do livro, que neste exemplo será **"LivroTeste"**:


```r
> newGitbook("LivroTeste");
```

Essa função irá criar a pasta **LivroTeste**, com os seguintes arquivos:
```
.bookignore
.gitignore
README.md
references.bib
references.Rmd
SUMMARY.md
```

+ ``README.md``: Página inicial do livro, contém o título e os autores do livro.
+ ``SUMMARY.md``: Especifica a estrutura do livro, também é o sumário do livro.

## Inicializando o Gitbook

2) O próximo passo da criação de um livro é a sua inicialização, ou seja, a função **initGitbook()** irá criar os arquivos R Markdown e suas respectivas pastas, especificadas no arquivo ``SUMMARY.md``:


```r
> initGitbook();
```

Essa função irá criar 2 pastas:

+ A **section1**, que contém os seguintes arquivos:

```
example1.Rmd
example2.Rmd
README.md
```

+ E a **section2**, que contém os seguintes arquivos:

```
example1.Rmd
README.md
```

Parabéns! Agora já temos alguns arquivos R Markdown que irão conter o texto do nosso livro.
