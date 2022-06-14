# Como adicionar o python no linux?
## UBUNTU 22.04 - PYTHON 3.10.4 
Para este tutorial será considerada a versão 3.10.5 do python, para ambientes de desenvolvimento baseado em debian, especialmente no Ubuntu.
Neste caso foi utilizado o Pop!OS 22.04 LTS, versão estável desenvolvida pela System76, baseado no Ubuntu 22.04 LTS.

OBSERVAÇÃO: É NECESSÁRIO SER ADMINISTRADOR PARA EXECUTAR COMANDOS SUDO, NÃO USE ESTE COMANDO DE FORMA IRRESPONSÁVEL VISTO QUE É UM COMANDO ROOT.
NÃO COPIE O $ APENAS O COMANDO!

1º  Abra o terminal, e digite os seguintes comandos de super-usuário, estes comandos são responsáveis por atualizar o seu sistema.
    
    $ sudo apt-get full-upgrade
    $ sudo apt-get update
    
2º  É importante checar a versão do python previamente instalada no seu linux.

    $ python3 --version

3º  Instale o git e o curl, para permitir futuras instalações de repositórios github.

    $ sudo apt install git curl

4º  Instale o pip, o python (caso não esteja instalado), o virtualenv, a idle python e todos os comandos abaixo.

    $ sudo apt install python3.10 python3.10-dev python3.8-venv 
    $ \python3-venv idle-python3.10 python3-pip virtualenv gcc 
    $ \default-libmysqlclient-dev libssl-dev -y

5º  Instale o gerenciador de pacotes snap caso não possua com os comandos abaixo. 
    
    $ sudo apt-get install snapd snapd-xdg-open
    
6º  Instale o pycharm, o virtual studio code e o atom com os comandos abaixo. O pycharm é a ide necessária para o aprendizado, os outros programas são editores.

    $ sudo snap install pycharm-community --classic
    $ sudo snap install --classic vscode
    $ sudo snap install atom
    
7º  Atualize os editores de texto e as ides instaladas.

    $ sudo snap refresh pycharm-community
    $ sudo snap refresh vscode
    $ sudo snap refresh atom
