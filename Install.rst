Installing Banzai
=================

We're only targeting Ubuntu 14.04 (at the moment).

You need root. 

Do something like this::

    #######################################
    # Update & install minimum requirements
    #######################################
    sudo apt-get update
    sudo apt-get install git build-essential python-pip python-dev openjdk-7-jre unzip zlib1g-dev libncurses5-dev libfreetype6-dev libfreetype6 libpng-dev pkg-config libcairo2-dev 

    sudo cpan -i JSON
    sudo cpan -i Cairo
    sudo cpan -i Statistics::PCA
    sudo perl -MCPAN -e "CPAN::Shell->notest('install', 'List::MoreUtils')"


    #################################
    # Install linuxbrew & tap recipes
    ################################
    git clone https://github.com/Homebrew/linuxbrew.git ~/.linuxbrew
    export PATH="$HOME/.linuxbrew/bin:$PATH"
    export MANPATH="$HOME/.linuxbrew/share/man:$MANPATH"
    export INFOPATH="$HOME/.linuxbrew/share/info:$INFOPATH"
    echo '' >> ~/.bashrc
    echo 'export PATH="$HOME/.linuxbrew/bin:$PATH"' >> ~/.bashrc
    echo 'export MANPATH="$HOME/.linuxbrew/share/man:$MANPATH"' >> ~/.bashrc
    echo 'export INFOPATH="$HOME/.linuxbrew/share/info:$INFOPATH"' >> ~/.bashrc
    echo '' >> ~/.bashrcbrew tap homebrew/science
    brew tap chapmanb/cbl
    brew tap tseemann/homebrew-bioinformatics-linux
    brew tap mscook/BanzaiNGS

    brew install Banzai
