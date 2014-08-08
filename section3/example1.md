
# Instalando o pacote RGitbook

Baixe e instale o [Node.js](http://nodejs.org/)
```
devtools::install_github("raulossada/Rgitbook");
require(Rgitbook);
```

***

2) Instale globalmente o `gitbook-plugin`
```
system("npm install gitbook-plugin -g");
```

Also, I had to manually download and install in the appropriate place the phantomjs-1.9.7-windows.zip from: http://phantomjs.org/download.html

***

3) Verifique se os módulos `npm` e `gitbook` estão instalados.
```
checkForGitbook();
```

***

4) Verifique se a última versão do módulo do `gitbook` está instalada.
```
gitbookInfo();
```

***

## Outra seção

5) Criando um novo livro
```
newGitbook("testbook");
```

***

## Outra seção

6) Inicialize o seu livro (O que quer dizer inicializar?).

Lê o arquivo SUMMARY.md da pasta e cria a estrutura/esqueleto do livro baseada nesse arquivo.
````
initGitbook();
````

***

## Outra seção

7) Crie/Atualize os arquivos `*.Rmd` a partir dos arquivos `*.md`
```
buildGitbook();
```

***

## Outra seção

8) Abra o seu livro num navegador web
```
openGitbook();
```
