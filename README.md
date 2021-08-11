<img src="img/git.png">

###### Obs: Informações tiradas do site: <a href = "https://www.atlassian.com/br/git/tutorials/what-is-git#performance">Bitbucket </a>.

# O que é Git

<a href = "#desempenho">Desempenho </a> |  <a href = "#seguranca">Segurança</a> | <a href = "#flexibilidade">Flexibilidade</a> | <a href = "#controle">Controle de versões com Git</a>

De longe, o sistema de controle de versão moderno mais usado no mundo hoje é o Git. O Git é um projeto de código aberto maduro e com manutenção ativa desenvolvido em 2005 por Linus Torvalds, o famoso criador do kernel do sistema operacional Linux. Um número impressionante de projetos de software depende do Git para controle de versão, incluindo projetos comerciais e de código-fonte aberto. Os desenvolvedores que trabalharam com o Git estão bem representados no pool de talentos de desenvolvimento de software disponíveis e funcionam bem em uma ampla variedade de sistemas operacionais e IDEs (Ambientes de Desenvolvimento Integrado).

Tendo uma arquitetura distribuída, o Git é um exemplo de DVCS (portanto, Sistema de Controle de Versão Distribuído). Em vez de ter apenas um único local para o histórico completo da versão do software, como é comum em sistemas de controle de versão outrora populares como CVS ou Subversion (também conhecido como SVN), no Git, a cópia de trabalho de todo desenvolvedor do código também é um repositório que pode conter o histórico completo de todas as alterações.

Além de ser distribuído, o Git foi projetado com desempenho, segurança e flexibilidade em mente.

<p id = "desempenho">

## Desempenho

As características brutas de desempenho do Git são muito fortes quando comparadas a muitas alternativas. Fazer o commit de novas alterações, branches, mesclagem e comparação de versões anteriores – tudo é otimizado para desempenho. Os algoritmos implementados no Git aproveitam o conhecimento profundo sobre atributos comuns de árvores de arquivos de código-fonte reais, como costumam ser modificados ao longo do tempo e quais são os padrões de acesso.

Diferente de alguns softwares de controle de versão, o Git não se deixa enganar pelos nomes dos arquivos ao determinar qual deve ser o armazenamento e o histórico de versões da árvore de arquivos. Em vez disso, o Git se concentra no conteúdo do arquivo. Afinal, os arquivos de código-fonte são renomeados, divididos e reorganizados com frequência. O formato do objeto dos arquivos de repositório do Git usa uma combinação de codificação delta (armazenamento de diferenças de conteúdo) e compactação e armazena com clareza o conteúdo do diretório e os objetos de metadados da versão.

A distribuição também oferece benefícios significativos de desempenho.

Por exemplo, digamos que uma desenvolvedora, Alice, faça alterações no código-fonte, adicionando um recurso para a próxima versão, 2.0, e faça o commit dessas alterações com mensagens descritivas. Ela então trabalha em um segundo recurso e faz o commit dessas alterações também. Como esperado, eles são armazenados como peças de trabalho separadas no histórico de versões. Alice então muda para o branch da versão 1.3 do mesmo software para corrigir um erro que afeta apenas a versão mais antiga. O objetivo disso é permitir que a equipe de Alice lance uma versão de correção de bug, a versão 1.3.1, antes que a versão 2.0 esteja pronta. Alice pode retornar ao branch 2.0 para continuar trabalhando nos novos recursos da versão 2.0. Tudo isso pode ocorrer sem nenhum acesso à rede e, portanto, é um processo rápido e confiável. Ela poderia até fazer isso em um avião. Quando estiver pronta para fazer o commit de todas as alterações como itens individuais no repositório remoto, Alice vai poder enviar todas elas por push em um único comando.

</p>

<p id = "seguranca">

## Segurança

O Git foi projetado com a integridade do código-fonte gerenciado como uma prioridade. O conteúdo dos arquivos, bem como os verdadeiros relacionamentos entre arquivos e diretórios, versões, tags e commits, todos esses objetos no repositório do Git são protegidos com um algoritmo de hash de criptografia seguro chamado SHA1. Isso protege o código e o histórico de alterações contra alterações acidentais e maliciosas e garante que o histórico tenha rastreabilidade total.

Com o Git, você pode ter certeza de ter um histórico de conteúdo autêntico do código-fonte.

Alguns outros sistemas de controle de versão não têm proteções contra alterações secretas posteriores. Isso pode ser uma vulnerabilidade séria de segurança das informações para qualquer empresa que depende do desenvolvimento de software.

</p>

<p id = "flexibilidade">

## Flexibilidade

Um dos principais objetivos de design do Git é a flexibilidade. O Git é flexível em vários aspectos: suporte a vários tipos de fluxos de trabalho de desenvolvimento não lineares, em eficiência em projetos pequenos e grandes e em compatibilidade com muitos sistemas e protocolos existentes.

O Git foi projetado para tratar os branches e tags como cidadãos de primeira classe (ao contrário do SVN) e operações que afetam branches e tags (como mesclagem ou reversão) também são armazenadas como parte do histórico de alterações. Nem todos os sistemas de controle de versão apresentam esse nível de rastreamento.

<p id = "controle">

## Controle de versões com Git

Hoje, o Git é a melhor escolha para a maioria das equipes de software. Embora cada equipe seja diferente e deva fazer a própria análise, aqui estão os principais motivos pelos quais o controle de versão com Git é preferido em vez de alternativas:

### O Git é bom

O Git tem a funcionalidade, desempenho, segurança e flexibilidade que a maioria das equipes e desenvolvedores individuais precisa. Esses atributos do Git são explicados acima. Nas comparações lado a lado com a maioria das outras alternativas, muitas equipes acham que o Git é muito favorável.

### Git é um padrão de fato

O Git é a ferramenta mais adotada da categoria. Ele é atraente pelos seguintes motivos. Na Atlassian, quase todo código-fonte do projeto é gerenciado no Git.

Um grande número de desenvolvedores já tem experiência com o Git e uma proporção significativa de recém-formados pode ter experiência apenas com o Git. Embora algumas empresas precisem escalar a curva de aprendizado ao migrar para o Git de outro sistema de controle de versão, muitos desenvolvedores existentes e futuros não precisam ser treinados no Git.

Além dos benefícios de um grande conjunto de talentos, a predominância do Git também significa que muitas ferramentas e serviços de software de terceiros já estão integrados ao Git, incluindo IDEs e novas ferramentas de uso como o cliente de desktop DVCS [Sourcetree](http://www.sourcetreeapp.com/br/), software de rastreamento de itens e projetos, [Jira](https://www.atlassian.com/br/software/jira), e serviço de hospedagem de código, [Bitbucket](https://bitbucket.org/product/br/).

Se você é um desenvolvedor inexperiente que quer desenvolver habilidades valiosas em ferramentas de desenvolvimento de software, quando se trata de controle de versão, o Git deve ser um dos itens na lista.

### Git é um projeto de código aberto de qualidade

O Git é um projeto de código aberto muito bem suportado, com mais de uma década de administração sólida. Os mantenedores do projeto mostraram um julgamento equilibrado e uma abordagem madura para atender às necessidades de longo prazo dos usuários, com lançamentos regulares que melhoram a usabilidade e a funcionalidade. É fácil examinar a qualidade do software de código aberto, e inúmeras empresas dependem muito dessa qualidade.

O Git tem excelente suporte da comunidade e uma vasta base de usuários. A documentação é excelente e abundante, incluindo livros, tutoriais e sites dedicados. Existem também podcasts e tutoriais em vídeo.

O código aberto reduz o custo para desenvolvedores amadores, pois eles podem usar o Git sem pagar uma taxa. Para uso em projetos de código aberto, o Git é sem dúvida o sucessor das gerações anteriores de sistemas bem-sucedidos de controle de versão de código aberto, SVN e CVS.

### Crítica ao Git

Uma crítica comum ao Git é que pode ser difícil de aprender. Algumas das terminologias do Git vão ser novas para os iniciantes e, para usuários de outros sistemas, a terminologia do Git pode ser diferente, por exemplo, `revert` no Git tem um significado diferente do que no SVN ou CVS. No entanto, o Git é muito capaz e disponibiliza muitos recursos aos usuários. Aprender a usar esses recursos pode levar algum tempo. No entanto, uma vez aprendidos, podem ser usados pela equipe para aumentar a velocidade de desenvolvimento.

Para as equipes que vêm de um VCS não distribuído, ter um repositório central pode parecer uma coisa boa que eles não querem perder. No entanto, embora o Git tenha sido projetado como um sistema de controle de versão distribuído (DVCS), com o Git, você ainda pode ter um repositório canônico oficial em que todas as alterações no software devem ser armazenadas. Com o Git, como o repositório de cada desenvolvedor está completo, o trabalho não precisa ser restringido pela disponibilidade e desempenho do servidor "central". Durante interrupções ou quando offline, os desenvolvedores ainda podem consultar o histórico completo do projeto. Como o Git é flexível e está sendo distribuído, você pode trabalhar da maneira que está acostumado, mas obter os benefícios adicionais do Git, alguns dos quais você nem percebe que está perdendo.

Agora que você entende o que é o controle de versão, o que é o Git e por que as equipes de software deveriam optar por ele, continue lendo para descobrir os benefícios que o Git pode oferecer em toda a empresa.

</p>

# Instalar o Git

Antes de utilizarmos o Git, precisamos instalá-lo no Sistema Operacional que usamos.

<a href = "#windows">Windows</a> | <a href = "#linux">Linux</a> | <a href = "#mac">Mac OS</a>

<p id = "windows">

## Windows

   1. Baixe o instalador mais recente do [Git](https://git-scm.com/downloads).

   2. Quando você tiver iniciado o instalador com sucesso, vai ver a tela do assistente de **configuração do Git**. Siga os avisos **Next** e **Finish** para concluir a instalação. As opções padrão são bastante sensíveis para a maioria dos usuários.

   3. Depois de ter instalado o git, abra o git bash, powershell ou o cmd do linux e verifique a versão do git para saber se está tudo certo:

      ```bash
      git --version
      ```

      ```bash
      git version 2.25.1
      ```

</p>

<p id = "linux">

## Linux

   ### Debian/Ubuntu/Linux Mint (apt-get)

   Para instalar o Git no linux, pode ser feito via linha de comando, basta usar o gerenciador de pacotes da distro que você está usando (No caso do Ubuntu ou derivados, o gerenciador de pacotes é o apt-get ou so apt).

   1. Abra seu terminal, e digite o comando para instalar o git usando o `apt`:

      ```bash
      sudo apt-get update
      ```

      ```bash
      sudo apt install git -y
      ```

   2. Verifique se a instalação foi bem-sucedida digitando:

      ```bash
      git --version
      ```

      ```bash
      git version 2.25.1
      ```

   ### Fedora(dnf/yum)

   1. Abra seu terminal, e digite o comando para instalar o git usando o `dnf`:

      ```bash
      sudo dnf update
      ```

      ```bash
      sudo dnf install git -y
      ```

   2. Verifique se a instalação foi bem-sucedida digitando:

      ```bash
      git --version
      ```

      ```bash
      git version 2.25.1
      ```

</p>

<p id = "mac">

## Mac OS

   A maneira mais fácil de instalar o Git em um Mac é por meio do instalador autônomo:

   1. Faça download do instalador mais recente do [Git](https://git-scm.com/downloads).

   2. Siga os avisos para instalar o Git.

   3. Abra um terminal e verifique se a instalação foi bem-sucedida digitando o código `git --version`:

      ```bash
      git --versão
      ```

      ```bash
      git version 2.25.1
      ```

### Instalar o Git com Homebrew

   Se tiver [instalado o Homebrew](http://brew.sh/) para gerenciar pacotes no OS X, siga estas instruções para instalar o Git:

   1. Abra seu terminal e instale o Git usando Homebrew:

      ```bash
      $ brew install git
      ```

   2. Verifique se a instalação foi bem-sucedida digitando a `git --version`:

      ```bash
      $ git --version 
      ```

      ```bash
      git version 2.25.1
      ```

</p>

## Configurações iniciais do Git

Depois de ter instalado o Git, uma das primeiras coisas que devemos fazer é configurar ele com o seu nome de usuário e e-mail do Git, com os comandos a seguir:

```bash
git config --global user.name "Seu usuário"
```

```bash
git config --global user.email "seu_email@gmail.cm"
```

#### Exemplo:

```bash
git config --global user.name "Emma Paris"
```

```bash
git config --global user.email "emmaparis@gmail.cm"
```

Essas informações vão ser associadas a quaisquer commits que você criar. Caso você queira configurar seu editor de código também, basta digitar:

```bash
git config --global core.editor nome_do_editor
```

#### Exemplo:

```bash
git config --global core.editor code
```

Ele vai definir o Visual Studio Code como editor padrão do seu Git. Para ver todas as suas configurações definidas no Git, basta digitar:

```bash
git config --list
```
