
# Publicando um GitBook

Nesta seção, vamos ver quais são os comandos que a função **publishGitbook()** usa para publicar um **GitBook** pronto no servidor do **GitHub**.

Iremos ver estes comandos, pois até a data de 11/Agosto/2014, a função apresentou alguns problemas para funcionar no RStudio do Windows e do Linux. Assim sendo, tenha tenha certeza de estudar bem os passos a seguir antes de tentá-los.

(**Atenção!** Se você quiser publicar o livro no servidor do **GitBook**, recomenda-se utilizar o [Book Editor do GitBook](https://www.gitbook.io/) para fazer isso).

***

1) Abra o **Git Shell** e mude o seu diretório para a pasta **_book** do seu livro:

```
cd {{CaminhoAtéAPasta}}/_book
```

2) Crie um repositório Git local:

```
git init
```

3) Faça um **Commit**:

```
git commit --allow-empty -m 'Update built gitbook1'
```

4) Crie um novo galho (do inglês, *Branch*) e mude para ele:

```
git checkout -b gh-pages
```

5) Adicione o conteúdo da pasta ao índice para fazer um **Commit**:

```
git add .
```

6) Faça um **Commit** para esse novo galho:

```
git commit -a -m 'Update built gitbook2'
```

7) Publique o livro no servidor do GitHub:

```
git push https://github.com/{{UsuárioDoGitHub/NomeDoRepositório}} gh-pages --force
```

Com sorte, o livro foi publicado no servidor do GitHub. Parabéns!
