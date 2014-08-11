
# Instalando o pacote Rgitbook

Antes de instalarmos o Rgitbook, temos que instalar outros softwares que são pré-requisitos para que o Rgibook funcione corretamente:

1) Baixe e instale o [Node.js](http://nodejs.org/).

2) Abra o **RStudio** e instale o pacote ``devtools``, que possui uma função para instalar pacotes diretamente do GitHub:


```r
> install.packages("devtools");
```

3) Instale e carregue o pacote ``Rgitbook`` no RStudio.

**Atenção!** Até a data de 11/Agosto/2014, o pacote Rgitbook apresentava alguns problemas que não haviam sido corrigidos no repositório original (jbryer/Rgitbook), contudo, a versão usada no código abaixo já tem as devidas correções, e já foi feito um **Pull Request** para que estas correções sejam incorporadas no repositório original:


```r
> devtools::install_github("raulossada/Rgitbook");
> require("Rgitbook");
```

4) No RStudio, desinstale a instalação local do ``gitbook-plugin`` e instale-o globalmente usando o seguinte código:


```r
> system("npm uninstall gitbook-plugin");
> system("npm install gitbook-plugin -g");
```

5) Caso apareça alguma mensagem de erro pedindo para você instalar o ``phantomjs``. Você pode baixá-lo daqui: [phantomjs-1.9.7-windows](http://phantomjs.org/download.html) e instalá-lo manualmente no local apropriado.

6) Verifique se os módulos ``npm`` e ``gitbook`` foram instalados:


```r
> checkForGitbook();
```

7) Verifique se a última versão do módulo do ``gitbook`` está instalada:


```r
> gitbookInfo();
```

Parabéns! Acabamos de instalar o Rgitbook!
