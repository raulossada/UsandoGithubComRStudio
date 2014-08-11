
# Construindo/Atualizando os arquivos Markdown

1) Continuando a criação do livro, agora iremos usar a função **buildGitbook()** para criar arquivos Markdown (\*.md), a partir dos arquivos R Markdown (\*.Rmd):


```r
> buildGitbook();
```

+ Essa função cria a pasta **_book**, que contém os arquivos *.html da versão Website do livro. E os arquivos:

```
.rmdbuild
references.md

section1/example1.md
section1/example2.md

section2/example1.md
```

**Importante!**: Essa função também serve para atualizar os arquivos Markdown quando você editar os arquivos R Markdown.

**Muito importante!!!**: Sempre que você for modificar o conteúdo do livro, sempre edite os arquivos R Markdown (\*.Rmd), pois eles são à base para a construção dos arquivos Markdown (\*.md) quando se usa o pacote ``Rgitbook``. Os únicos arquivos que fogem á essa regra são os ``README.md`` e o ``SUMMARY.md``, já que não possuem um equivalente R Markdown e portanto podem ser editados diretamente.
