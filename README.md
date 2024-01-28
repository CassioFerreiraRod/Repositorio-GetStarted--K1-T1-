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
Copy code
git pull origin nome_do_branch
~~~
Para mesclar as alterações de um branch:

~~~bash
Copy code
git merge nome_do_branch
~~~
**Enviando Alterações para o Repositório Remoto**

Envie alterações para o repositório remoto com:

~~~bash
Copy code
git push origin nome_do_branch
~~~
Estes são comandos básicos do Git. Consulte a documentação oficial do Git para obter informações detalhadas.
