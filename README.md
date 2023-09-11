# Setup Anaconda on a Mac

## Install Homebrew
Run the following command on your terminal to install Homebrew. 
Homebrew is a package manager for Macs and is used to install useful development tools and software.

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

## Install Anaconda through Homebrew
1. Run `brew install --cask anaconda` to install Anaconda
2. Run `echo 'export PATH=/usr/local/anaconda3/bin:$PATH' >> ~/.zshrc` from your terminal
3. Also run `echo 'export PATH=/opt/homebrew/anaconda3/bin:$PATH' >> ~/.zshrc` from your terminal
4. Run `source ~/.zshrc` from your terminal
5. Type `conda` to ensure that anaconda linked correctly.

#### If you use bash instead of zsh, replace steps 2 and 3 from above with the following:
- `echo 'export PATH=/usr/local/anaconda3/bin:$PATH' >> ~/.bash_profile`
- `echo 'export PATH=/opt/homebrew/anaconda3/bin:$PATH' >> ~/.bash_profile`
- `source ~/.bash_profile`

![Setup Anaconda On Macbook (M1/M2)](/img1.png "Setup Anaconda On Macbook")

## If you've already installed anaconda from the installation file from anaconda.org
If you installed Anaconda for only this user, run the following:
- `echo 'export PATH=/Users/$USER/anaconda3/bin:$PATH' >> ~/.zshrc`
- `echo 'export PATH=/opt/homebrew/anaconda3/bin:$PATH' >> ~/.zshrc`
- `source ~/.zshrc`

If you installed Anaconda for all users on your computer, then run the following:
- `echo 'export PATH=/opt/anaconda3/bin:$PATH' >> ~/.zshrc`
- `source ~/.zshrc`