*************
Git e Git-Hub
*************
| O Git é um programa usado localmente em um computador para desenvolvimento e versionamento de códigos.
| O Git-Hub é uma plataforma de desenvolvimento para guardar os projetos versionados. Concorrentes: GitLab, BitBucket, entre outros.
Acessando o Git localmente
==========================
| Em Windows, deve ser instalado anteriormente em https://git-scm.com/download/win , em Linux já é nativo.
| **1)** Linux - acessar Git pelo Terminal digitando:
|  ``git``
|
| **2)** Entrar na pasta onde mexerá nos repositórios utilizando:
| ``cd <endereço_da_pasta>``
Acessando o Git-Hub via web
===========================
| **1)** Acessar sua conta Git-Hub pelo navegador
|
| **2)** Ir no repositório que deseja fazer alterações
|
| **3)** Copiar link do repositório que deseja alterar

Clonando seu repositório Git-Hub localmente no Git
==================================================
| **1)** Para fazer as alterações no arquivos que deseja, primeiramente deve-se clonar localmente o repositório onde localizam-se esses arquivos, executando no terminal o comando:
| ``git clone <link_do_repositório>``
|
| **2)** Entre no terminal na pasta criada do repositório com o comando:
| ``cd <endereço da pasta>``
|
| **3)** Lá utilize o comando:
| ``git status``
| Este é o comando para saber a situação de versionamento de seu projeto

Formatando arquivos e versionando (*commit*) para o Git-Hub
=========================================================
| **1)** Os arquivos de anotações podem ser criados em formato .txt e .str
| Os arquivos .str tem melhor visualização, já que existem alguns caracteres que podem ser colocados no arquivos para sua melhor visualização no Git-Hub
| **2)** Dê um ``git status`` para verificar seu projeto
| **3)** Agora para indicar que quer que seu arquivo seja versionado dê o comando:
| ``git add <nome do arquivo>``
| **4**) Para verificar o histórico de versionamento do arquivo utilize:
| ``git log``
| **5)** Para fazer o versionamento (*commit*) para o Git-Hub utilize:
| ``git commit -a`` -> vai para um editor dentro do terminal que você pode adicionar comentários sobre o arquivo que está versionando
| **ou**
| ``git commit -m "mensagem que quero enviar"`` -> faz o processo anterior em uma linha só
| **6)** Dê ``git status`` ou ``git log`` para verificar se seu versionamenro (commit) foi feito

Atualizando o Git-Hub do projeto
================================
| **1)** Para enviar as alterações (*commits*) feitas localmente para o Git-Hub dê o comando:
| ``git push <nome do diretório mestre (master)>``

Criando *issues* e *tickets*
============================
| Ao produzir projetos em grupo, melhorias em projetos são sugeridas através da aba *Issues* dentro do Git-Hub
| **1)** Acesse no Git-Hub ``<link do documento a ser comentado/issues>``
| **2)** Fazer uma *Issue* do projeto. Uma *issue* tem que ser algo único, não uma lista. Os issues recebem números, dessa forma quando corrigir no código algo relacionado à um *issue* você pode atribuir o número da *issue*.

Criando novos ramos (branch)
=============================
| Até agora, tudo foi feito o ramo mestre (*branch master*). Agora com um *issue* criado, pode-se fazer uma *branch* para esse *issue*.
| **1)** Digite ``git branch`` para ver quais os ramos existentes
| **2)** Para criar um novo ramo use:
| ``git branch <nome_do_ramo>``
| **3)** Para mover de ramo use:
| ``git checkout <nome_do_ramo>``
| **3.1)** Pode-se criar e mover para um novo ramo em um único comando usando:
| ``git checkout -b <nome_do_ramo>``
|
`

Unindo arquivos do issue com arquivo do ramo master
===================================================
| **1)** Selecione *Pull request*
| **2)** E selecione *Merge*

Atualizando no terminal Git o merge feito no Git-Hub
====================================================
| **1)** Mude para ramo master com:
| ``git branch <nome_do_ramo>``
| **2)** Atualize o ramo master com:
| ``git pull <link do diretório do trabalho>``

Fazendo trabalhos colaborativos
===============================
| **1)** Vá no repositório da pessoa que irá colaborar no Git-Hub
| **2)** Clique no topo do lado direito em:
| Nota Importante: *Fork*
| O *fork* é uma cópia de um projeto (o que está no master ou um *branch default*, por exemplo, v3.0) que você poderá editar localmente. Um exemplo: vamos supor que eu criei um projeto *open source* (código aberto) chamado ProjetoX. Então, se você se interessa em contribuir, então você faz o *fork* de meu projeto. Então, você terá uma cópia exata do que está no ProjetoX naquele momento em que fez o *fork*. Tudo o que você fizer deve ficar no seu *fork*. Quando achar que tem uma contribuição para o projeto, você faz um *pull request* para o meu projeto sinalizando sua contribuição, para que eu possa aceitá-la ou não. Outra possiblidade é você nunca fazer o *pull request*, simplesmente desenvolver o seu projeto a partir de um existente, criando um novo produto.
| **3)** A partir daí é só utilizar todos os comando utilizados anteriormente para alterações e realizar um pull request.
