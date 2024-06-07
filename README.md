# Bootcamp Santander/AdaTech - Git/Versionamento

## Esta é uma apostila de comandos do Git que já utilizei, e que achei interessante, junto com uma explicação do que cada um faz.

### Estados do GIT

Antes de começarmos a falar dos comandos do Git, é necessário falar sobre os tipos de estados dos arquivos do Git.

Existem 4 tipos:

1. **Untracked**: É quando o arquivo ainda não foi mapeado pelo git;
2. **Unmodified**: É quando o arquivo já foi mapeado por git, ou seja, já ocorreu commit e passou pelo estado "staged";
3. **Modified**: É quando o arquivo foi editado e salvo;
4. **Staged**: É quando o arquivo está pronto para receber o commit e subir no repositório remoto.

##

### Comandos do Git

* **git init**: Inicia o git no diretório local;

* **git config --global user.name "*seu_nome*"**: Configura o seu nome para que fique salvo nos commits;

* **git config --global user.email *seu_email@email.com***: Configura o seu email para que fique salvo nos commits;

* **git branch -M main**: Cria uma branch main para subir os commits;

* **git add *nome_do_arquivo***: Irá mudar o estado do arquivo de "modified" para "staged";

* **git commit -m "*mensagem*"**: Faz um commit no arquivo com a mensagem que desejar;

* **git clone *url***: Copia um diretório remoto informado no diretório local atual;

* **git remote add origin *url***: Conecta o diretório local atual com o diretório remoto informado;

* **git push -u origin main**: Publica os commits feitos na branch main, no caso, no diretório remoto;

* **git diff**: Apresenta no terminal as linhas que foram alteradas com um visão de como era antes e como está atualmente de um arquivo do estado "modified";

* **git diff --staged**: Apresenta no terminal as linhas que foram alteradas de como era antes e como está atualmente de um arquivo do estado "staged";

* **git log**: Apresenta no terminal todos os commits realizados até o momento com a "hash", onde é salvo para o git quando é necessário retornar o código como estava antes do commit mais recente;

* **git log --oneline --decorate**: Apresenta no terminal a primeira de todos os commits realizados até o momento;

* **git restore**: Retorna o código para como era antes da modificação mais recente sem ter executado o git add;

* **git restore --staged *nome_do_arquivo***: Retorna o código para como era antes da modificação mais recente após executar o git add;

* **git status**: Retorna no terminal os estados de todos os arquivos do diretório atual;

* **git status *nome_do_arquivo***: Retorna no terminal o estado do arquivo informado do diretório atual;

* **git pull**: Coleta todas as informações que estavam no diretório remoto, compara com o diretório local e caso esteja desatualizado o local, os dados são atualizados conforme o remoto;

* **git fetch**: Coleta todas as informações que estavam no diretório remoto e baixa no diretório local, mas sem inserir no código ainda. Após executar este comando, execute o git diff para validar o que está faltando no local e que será atualizado com base no remoto antes de executar o git pull;

* **git branch**: Lista todas as branchs do diretório e diferencia a branch atual;

* **git branch *nome_da_branch***: Cria uma nova branch;

* **git checkout *nome_da_branch***: Acessa a branch informada;

* **git merge *nome_da_branch***: Leva as informações da branch informada para a branch atual.
