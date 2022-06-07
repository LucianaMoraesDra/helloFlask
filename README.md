# helloFlask
    1) Installation des dépendances :
    
    sudo apt-get update; sudo apt-get install make build-essential libssl-dev zlib1g-dev \    libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm \    libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
    
    2) Installer Pyenv :
    curl https://pyenv.run | bash
    
    3 ) Rajouter dans le fichier .bashrc les lignes suivantes :
    
    4) Commenter le bloc conda initialize pour éviter tout conflit avec Pyenv
    *Load pyenv automatically
    export PYENV_ROOT="$HOME/.pyenv" 
    command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"
    eval "$(pyenv init -)"
    *Load pyenv-virtualenv automatically
    eval "$(pyenv virtualenv-init -)"
    
    5) Création d'un environnement conda avec miniconda :
    pyenv install --list    pyenv install miniconda3-4.7.12    pyenv versions
    
    6) Activation de l'environnement conda :
    pyenv activate miniconda3-4.7.12
    
    7) Installation d'une version de Python :
    pyenv install 3.10.4
    pyenv virtualenv 3.10.4 testEnv310
    
    8) Lister les différents environnements dispo :
    pyenv virtualenvs
    
    9) Activé l'environnement virtuel
    pyenv activate testEnv310
    
    10) Définir la version comme interpréteur global:
    pyenv global 3.10.4    python --version
    
    11) Définir la version comme interpréteur local :
    pyenv install 2.8.6
    pyenv local 2.8.6
    python --version
    
    
    
    
    __text by Mathieu GUIGNET__
