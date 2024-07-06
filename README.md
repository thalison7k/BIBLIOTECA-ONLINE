biblioteca-pi1
Bem vindo a Biblioteca Social de Capela do Alto, este site foi desenvolvido para a disciplina de projeto integrador I do eixo de Computação da Univesp. E tem como objetivo promover a leitura por meio do compartilhamento de livros nas escolas.

Configurando o ambiente (ubuntu)
Execute os comando abaixo no terminal:

sudo apt install python3-pip sudo pip3 install virtualenvwrapper

Adicionar as linhas abaixo no arquivo .bashrc no diretório home

export WORKON_HOME=$HOME/.virtualenvs
export VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3
export VIRTUALENVWRAPPER_VIRTUALENV_ARGS=' -p /usr/bin/python3 '
export PROJECT_HOME=$HOME/Devel
source /usr/local/bin/virtualenvwrapper.sh
Execute:

source ~/.bashrc

Criar o ambiente e instalar Django:

mkvirtualenv nome_ambiente pip3 install django

Rodar o projeto localmente :
Abra a pasta do projeto no terminal e execute:

pip3 install -r requirements.txt
python3 manage.py runserver
Abra o link http://127.0.0.1:8000 no navegador.
