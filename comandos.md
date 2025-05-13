Comandos:

git init
        Esse comando é para iniciar um novo repositorio na nossa máquina 
        Sempre que for iniciar um novo repositorio, faça isso dentro de uma pasta especifica para aquele repositorio.
        Criará arquivos dentro dessa pasta que serão sobre o repositorio e onde tudo acontece.

git add "nome do arquivo"
git add .
        O Comando ''git add'' serve para decidir quais arquivos serão commitados para o repositorio, exemplo:
        Você tem um projeto que tem vários arquivos e fez alterações em vários diferentes, mas só quer commitar um desses arquivos
        Então você usará o "git add "nome do arquivo" " para commitar apenas aquele arquivo.
        Se você deseja commitar todos os arquivos, você pode usar o comando "git add ." com um ponto final, que serão preparados todos os arquivos para serem commitados.

        Commitar - é um verbo criado na linguagem informal, para falar que os arquivos estão sendo inseridos no nosso repositorio.

git commit -m "nome do commit"
        Esse comando, é o comando que de fato vai inserir os arquivos no nosso repósitorio.
        Você pode dar o nome que quiser para esse commit, como "primeiro commit", "versão 0.0.1" e etc

git branch -M
        Esse comando é o comando que irá alterar o nome da "branch" que estamos mexendo no nosso repositorio.

git branch -M "main"
        É considerado boa prática alterar o nome da nossa branch "master" para "main", que será nossa branch principal.

Branch é a "linha do tempo" que estamos mexendo no nosso código, por exemplo, se tivermos 2 desenvolvedores em nossa equipe, podemos ter duas branchs, uma para cada, para cada um ir desenvolvendo sua parte, ou, se tivermos 2 tarefas para fazer em nosso código, uma tarefa para adicionar um botão, e uma tarefa para adicionar um efeito de rolamento no site, podemos criar duas branchs separadas para fazer alterações do código focando nessas tarefas, naquela branch especifica criada pra isso. 
Isso é muito importante para sempre mantermos uma organização e entendimento sobre o código.

git remote add origin <link do repositório>
        Para passar o commit do meu repositório local (da minha máquina) para um repositório na plataforma do Github, usamos o git remote add origin <link do repositório>
        origin é o nome utilizado para referenciar o nosso repositório

git push
git push origin main
git push origin novobotao
git push -u
git push -u origin main
        O commit que damos na máquina não sobe automaticamente para a plataforma
        Para isso precisaremos empurrar, enviar para lá com o comando que está acima. 
        Se você tiver mais de uma branch você pode escrever o branch por exemplo:   git push -u origin novobotao
        Assim irá para o repositorio online as alterações na "branch" "novobotao"
        Mas para isso é necessário ter criado essa branch antes no seu repositorio local.
    O -u é usado apenas na primeira vez, depois pode dar o comando "git push" sem o U
    A palavra "origin" está se referenciando ao repositorio.

git checkout -b 
git checkout -b "novobotao"
        Para adicionar uma branch em nosso repositorio, esse é o comando
        Você pode dar o nome que quiser, esse "novo botão" foi um exemplo de nome.

git checkout 
git checkout main
git checkout novobotao
        Esse é o comando que você altera o branch que está usando para fazer alterações.
        Se no git bash você estiver na branch "novobotao" e quiser mudar a branch "main"
        Você usa o comando com "main" que a partir da li, as alterações serão feitas na branch main

git merge
git merge novobotao
        Caso você queria implementar as atualizações da branch "novobotao" na branch principal "main"
        Você deve no BASH ir para a branch "main" e usar o comando acima.
        O Comando MERGE ele é como se fosse uma "SOMA", ele adiciona todas as alterações da branch que você escolher, na branch que você está.
        Por exemplo, se eu estou na branch main, eu coloco o "merge novobotao", todas as alterações do "novobotao" irão para a branch "main".

CLONANDO UM REPOSITORIO DO GIT HUB
        Sempre que você entrar em um repositório, seja o seu ou o de qualquer outra pessoa, entre no github e no repositorio que quer clonar.

        Você irá copiar esse link e levar ele lá pro nosso terminal

        O comando para puxar o projeto para a sua máquina é o git clone https://github.com/rafaballerini/GitTutorial.git
Comando:

git clone
git clone "link do repositorio"

        Não é necessário criar um repositório antes disso, como fizemos anteriormente com o git init. Dessa vez, basta abrir o terminal e clonar o projeto e tudo aparecerá!

git pull
        Esse comando irá puxar todas as alterações feitas no repositório do Github para o seu repositório local
        Caso alguém tenha feito alguma alteração no projeto, e você queria trabalhar naquela alteração, você pode usar esse comando que irá baixar as alterações para sua máquina.


Fork
        Existe a ferramenta fork que serve para clonar um repositorio do github de outra conta, para a sua conta (online -- não na sua máquina), se você entra nesse repositorio online e clicar no botão "fork", automaticamente será clonado esse repositorio para sua conta no github.