*************
Git e Git-Hub
*************
| O git é um programa usado localmente em um computador para desenvolvimento e versionamento de códigos.
| O github é uma plataforma de desenvolvimento para guardar os projetos versionados. Concorrentes: GitLab, BitBucket, entre outros.

Acessando o Git localmente
==========================
| Windows deve ser instalado anteriormente em https://git-scm.com/download/win , em Linux já é nativo)
| **1)** Linux - acessar Git pelo Terminal digitando:
|  `git`
| **2)** Entrar na pasta onde mexerá nos repositórios utilizando:
| `cd <endereço_da_pasta>`

Acessando o Git-Hub via web
===========================
| **1)** Acessar sua conta Git-Hub pelo navegador
| **2)** Ir no repositório que deseja fazer alterações
| **3)** Copiar link do repositório que deseja alterar

Clonando seu repositório Git-Hub localmente no Git
==================================================
| **1)** Após isso no terminal usar:
| .. git clone <link_do_repositório>
| Isso clona o repositório localmente na pasta encontrada no seu computador
| **2)** Entre na pasta criada do repositório com o comando:
| .. cd
| **3)** Lá utilize o comando
| `git status`
| Este é o comando para saber a situação de versionamento de seu projeto

Formatando arquivos e versionando (commit) para o Git-Hub
=========================================================
| **1)** Os arquivos de anotações podem ser criado em formato .txt e .str
| Os arquivos .str tem melhor visualização melhor, já existem alguns caracteres que podem ser colocados no arquivos para sua melhor visualização no Git
| **2)** Dê um git status para verificar seu projeto
| **3)** Agora para indicar que quer que seu arquivo seja versionado dê o comando:
| ``git add``
| ``git log *Mostra o histórico de versionamento (commit)``
| **4)** Para fazer o versionamento (commit) para o Git-Hub fazer:
| git commit -a -> vai para um editor dentro do terminal que você pode adicionar comentários sobre o arquivo que está versionando
| **ou**
| git commit -m <"mensagem que quero enviar"> -> faz o processo anterior em uma linha só
| **Ctrl + L limpa a tela do terminal**
| **5)** Dê git status e git log para verificar se seu versionamenro (commit) foi feito

Atualizando o Git-Hub do projeto
================================
| **1)** Dê o comando:
| git push <nome do diretório mestre (master)
| *Empurrar (push) o arquivo do commit localmente para o Git-Hub*

Criando issues e ticket
=======================
| Ao produzir projetos em grupo, elhorias em projetos são sugeridas através da aba "Issues" dentro do Git-Hub
| **1)** Acesse no Git-Hub <link do documento a ser comentado/issues>
| **2)** Faz issue do projeto. Uma issue tem que ser algo único, não uma lista. Os issues recebem números, dessa forma quando corrigir no código algo relacionado à um issue você pode atribuir o número do issue. Isso será visto a seguir.

Criando novos ramos (branch)
=============================
| Até agora, tudo feito o ramo mestre (branch master). Agora qye um issue foi criado, faremos um branch para esse issue.
| **1)** Digite *git branch* para ver os ramos no seu Git
| **2.1)** Para criar um novo ramo use
seealso:: git branch <nome_do_ramo>
| **2.2)** Outro comando que pode ser usado é:
| git checkout -b <nome_do_ramo>
| Um comando para criar e entrar no branch
| **3)** Use:
| git checkout <nome_do_ramo>
| Para trocar de ramo

Unindo arquivos do issue com arquivo do ramo master
===================================================
| **1)** Selecione Pull request
| **2)** E selecione Merge

Atualizando no terminal Git o merge feito no Git-Hub
====================================================
| **1)** Mude para ramo master
| **2)** Atualize o ramo master com:
| git pull <link do diretório do trabalho>

Fazendo trabalhos colaborativos
===============================
| **1)** Vá no repositório da pessoa que irá colaborar no Git-Hub
| **2)** Clique no topo do lado direito em:
| Nota Importante: *Fork*
| O fork é uma cópia de um projeto (o que está no master ou um branch default, por exemplo, v3.0) em seu computador. Um exemplo: vamos supor que eu criei um projeto open source (código aberto) ProjetoX. Então, se você se interessa em contribuir, então você faz o *Fork* de meu projeto. Então, você terá uma cópia exata do que está no ProjetoX naquele momento em que fez o Fork. Tudo o que você fizer deve ficar no seu *Fork*. Quando achar que tem uma contribuição para o projeto, você faz um *Pull request* para o meu projeto, sinalizando sua contribuição para que eu possa aceitá-la ou não. Outra possiblidade é você nunca fazer o *Pull request*, simplesmente desenvolver o seu a partir de um existente, criando um novo produto.
| **3)** A partir daí é só utilizar todos os comando utilizados anteriormente para alterações e realizar um pull request.
