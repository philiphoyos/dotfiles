# Setup
- follow this guide
    - https://yduman.github.io/blog/wsl2-setup/ or
    - https://www.omgubuntu.co.uk/how-to-install-wsl2-on-windows-10
- In ubuntu
    1. `sudo apt-get update`
    2. `sudo apt-get install -y build-essential checkinstall`
    3.  ```bash
            sudo apt-get install -y libncursesw5-dev \
            libssl-dev libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev \
            libffi-dev zlib1g-dev wget curl llvm libncurses5-dev git xz-utils \
            tk-dev libffi-dev liblzma-dev python-openssl libreadline-dev libsqlite3-dev \
            unixodbc-dev

        ```
- SSH keys (new)
    1. Setup ssh key pair in Ubuntu using the following link: (evt. brug eget initials@pc-name
    2. https://gist.github.com/cybersamx/1ad243b47cb0ac6734d2
- SSH keys (existing)
    1. Copy keys using the following command
    
        `cp -r .ssh/ ~/.ssh`
- Add ssh public key to Azure
    1.	Use following command and copy key
       
        `cat ~/.ssh/id_rsa.pub`
    2. Add key to Azure
5.	Install PyEnv
    1.	Run the following command in Ubuntu
        
        `curl https://pyenv.run | bash`
6.	Install Poetry
    1. Run the following command in Ubuntu
        
        `curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -`

# Dependencies on new projects
1.	Install Python
    1.	Run the following command in Ubuntu

2. Pyenv install 3.X (newest version)
    1.	If existing project use:
        
        `pyenv install` (*.python.version*  is a requirement)
