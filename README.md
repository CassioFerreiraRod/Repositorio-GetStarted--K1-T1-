# Repositorio-GetStarted--K1-T1-

## Git

O Git é um sistema de controle de versão amplamente utilizado para rastrear as alterações em projetos de software. Aqui estão alguns dos comandos básicos para começar a trabalhar com o Git.

### Comandos básicos:
**Para informações do usuário**
~~~bash
 git config --global user.name "Seu Nome"
 git config --global user.email "seu@email.com"
 ~~~
**Para iniciar um repositório**
 ~~~bash
 git init
 ~~~
 **Para clonar um repositório remoto**
 ~~~bash
 git clone URL_do_Repositorio
 ~~~
 **Para adicionar e commitar alterações**
 ~~~bash
 git add nome_do_arquivo
 ~~~
Confirme alterações com:
~~~bash
 git commit -m "Mensagem do Commit"
~~~
**Branches**

Criar uma branch:
~~~bash
 git branch nome_do_branch
~~~
Mudar para uma branch:
~~~bash
 git checkout nome_do_branch
~~~
**Atualizando e Mesclando**

Para obter as últimas alterações do repositório remoto:

~~~bash
git pull origin nome_do_branch
~~~
Para mesclar as alterações de um branch:

~~~bash
git merge nome_do_branch
~~~
**Enviando Alterações para o Repositório Remoto**

Envie alterações para o repositório remoto com:

~~~bash
git push origin nome_do_branch
~~~
**Salvando temporáriamente na memória**

Para salvar temporariamente mudanças não confirmadas em um local seguro:
~~~bash
git stash 
~~~
**Reescrevendo o Histórico de Commits**

O comando git rebase permite reorganizar e otimizar o histórico de commits, proporcionando um fluxo de trabalho mais limpo e linear. Ao contrário do git merge, que cria commits de mesclagem, o git rebase modifica o histórico existente.

Comandos Básicos:
~~~bash
git rebase -i HEAD~n
~~~
**Fluxo de Desenvolvimento com Git Flow**

O Git Flow é uma abordagem popular para gerenciar o desenvolvimento de software usando o Git. Ele define um conjunto de regras e procedimentos para simplificar o processo de colaboração em projetos, especialmente em equipes maiores. Aqui estão os conceitos básicos do Git Flow:

**Branches Principais:**

**Master:**

A branch master representa a versão de produção do software.
É considerada estável e reflete o estado atual do software em produção.

**Develop:**

A branch develop é a base para o desenvolvimento contínuo.
Novas funcionalidades e correções são mescladas nesta branch antes de irem para produção.

**Branches de Suporte:**

**Feature:**

Branches feature/ são criadas para implementar novas funcionalidades.
Elas são mescladas na branch develop quando a funcionalidade está completa.
Release:

Branches release/ são criadas para preparar uma versão para produção.
Correções de última hora e ajustes podem ser feitos nesta branch antes de ser mesclada em master e develop.

**Hotfix:**

Branches hotfix/ são usadas para corrigir problemas críticos em produção.
São mescladas em master e develop para garantir que as correções estejam presentes em ambas.

**Comandos Básicos:**

Iniciar o Git Flow:
~~~bash
git flow init
~~~

Iniciar uma Nova Feature e concluir:
~~~bash
git flow feature start nome_da_feature

git flow feature finish nome_da_feature
~~~

Iniciar e concluir uma Nova Release:
~~~bash
git flow release start nome_da_feature

git flow release finish nome_da_feature
~~~

Iniciar um Hotfix:
~~~bash
git flow hotfix start nome_da_feature

git flow hotfix finish nome_da_feature
~~~

Estes são comandos básicos do Git. Consulte a [documentação](https://git-scm.com/docs/git/pt_BR) oficial do Git para obter informações detalhadas.
