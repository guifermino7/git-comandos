# Bootcamp Santader/AdaTech - Git/Versionamento

## Esta é uma apostila de comandos do Git que já utilizei, e que achei interessante, junto com uma explicação do que cada um faz.


### Comandos do Git:

* **git init**: Inicia o git no diretório local;

* **git config --global user.name "*seu_nome*"**: Configura o seu nome para que fique salvo nos commits;

* **git config --global user.email *seu_email@email.com***: Configura o seu email para que fique salvo nos commits;

* **git add README.md**: Cria o arquivo "README.md" no diretório atual;

* **git branch -M main**: Cria uma branch main para subir os commits;

* **git add *nome_do_arquivo***: Irá mudar o estado do arquivo de "modified" para "staged";

* **git commit -m "*mensagem*"**: Faz um commit no arquivo com a mensagem que desejar;

* **git clone *url***: Copia um diretório remoto informado no diretório local atual;

* **git remote add origin *url***: Conecta o diretório local atual com o diretório remoto informado;

* **git push -u origin main**: Publica os commits feitos na branch main, no caso, no diretório remoto;

* **git diff**: Apresenta no terminal as linhas que foram alteradas com um visão de como era antes e como está atualmente de um arquivo do estado "modified";

* **git diff --staged**: Apresenta no terminal as linhas que foram alteradas de como era antes e como está atualmente de um arquivo do estado "staged";

* **git log**: Apresenta no terminal todos os commits rralizados até o momento com a "hash", onde é salvo para o git quando é necessário retornar o código como estava antes do commit mais recente;

* **git restore**: Retorna o código para como era antes da modificação mais recente sem ter executado o git add;

* **git restore --staged *nome_do_arquivo***: Retorna o código para como era antes da modificação mais recente após executar o git add.