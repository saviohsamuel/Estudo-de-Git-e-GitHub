mkdir (make directory) - criar diretório, cria um arquivo, seja ele uma pasta ou arquivo único.
    exemplo: mkdir projeto-1

ls (list) - dentro do meu diretório principal (estudo de git e GitHub) vai aparecer os dois diretórios que tem, ou seja, projeto-1 e projeto-2

mv (move) - usado para mover ou renomear arquivos e pastas
    exemplo: mv projeto-1 projeto-01

    explicação para renomear:
        primeiro nome (projeto-1) significa que quero renomear esse arquivo
        segundo nome (projeto-01) é o novo nome que será atribuido

    💡 Lembrando: o mv também serve para mover, dependendo se o segundo argumento for um diretório:        
        mv projeto-01 /home/savio/projetos/
        ➡️ Aqui ele move a pasta projeto-01 para dentro de /home/savio/projetos/.

cd .. (dois pontos)
    usando .. (dois pontos) é usando para retornar para o diretório anterior.

git init
    inicializa o repositório para começar a ser rastreado

cd projeto-02
    acessa o diretório passado logo depois do cd

touch nome-do-arquivo
    exemplo: touch index.html - cria um arquivo html no diretório que está atualmente.

git status
    verifica a situação dos arquivos para saber se já estão sendo rastreados, comitados etc.

    $ git status
        On branch master -→ você está no branch principal (master ou main).

        No commits yet -→ ainda não há nenhum commit no repositório.

        Untracked files: -→ arquivos que existem na pasta, mas o Git ainda não está rastreando.

            (use "git add <file>..." to include in what will be committed) - mostra o comando para começar a rastrear esses arquivos

            index.html -→ nome do arquivo que o Git detectou, mas ainda não foi adicionado.

            nothing added to commit but untracked files present (use "git add" to track)

git add nome-do-arquivo
    ➡️ Adiciona o arquivo à staging area (área de preparação) — ou seja, marca o arquivo para ser incluído no próximo commit.

    se fizer o comando git status vai exibir que tem um novo arquivo em staging area (área de preparação) para ser comitado

git add . (ponto)
    usado dessa forma para selecionar todos os arquivos para o staging area (área de preparaçao) para ser comitado

git commit -m "Descrição"
    serve para adicionar um comentário de uma modificação que foi realizada

git log
    exibe todos os commits, com muitas informações: hash completo, nome do autor, data e mensagem (commit)

git log --oneline
    mostra uma forma mais resumida do histórico de alterações
    exibe: hash abreviado e mensagem (commit)