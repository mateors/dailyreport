# dailyreport
Everyday is my new day

## Multiple github account

> touch ~/.ssh/config 

> nano ~/.ssh/config

```
# Home account
  Host home.github.com
  HostName github.com
  PreferredAuthentications publickey
  IdentityFile ~/.ssh/github

# Company account
  Host company.github.com
  HostName github.com
  PreferredAuthentications publickey
  IdentityFile ~/.ssh/id_ed25519
  
```
### Add ssh key
> ssh-add ~/.ssh/github

### Test your connection
> ssh -T git@home.github.com

> ssh -T git@company.github.com

### Now all are set, just clone your repositories
* repo -> https://github.com/mateors/dailyreport.git

> git clone git@home.github.com:mateors/dailyreport.git 

## Resource
* [how to add ssh key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
