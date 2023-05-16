# Master_The_Git by TheAbhiPatel

## How to setup ssh key in ubutu 
### 1. very first step 
* go in to the home directory and then .ssh directory 
  - Ex. cd  - for home directory
       cd .ssh - for go into the .ssh directory
* generate the ssh key with different algorithams from which you want
  - Ex. ssh-keygen -t ed25519 -b 4096 -C "user@domain.com" -f key-name
* you have received two file for key one is private key ex. (key-name) and second one is ex. (key-name.pub)
* edit your config file following staps 
* run command "gedit config" in your terminal
* edit config file like this
  -  Host bitbucket.org-username
     HostName bitbucket.org
     User git
     IdentityFile ~/.ssh/new-key
     IdentitiesOnly yes
* provide your public key to the host 
* with that finished your setup

### 2. add git config 
* by git command 
  Ex. - git config user.name "User name"
      - git config user.email "user@domain.com"
* by edit the git config by command given below
 Ex. - git config --global --edit
        
