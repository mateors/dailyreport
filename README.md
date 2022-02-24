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

> ssh-add ~/.ssh/github

> ssh -T git@home.github.com

> ssh -T git@company.github.com

### Github repo
* https://github.com/mateors/dailyreport.git

> git clone git@home.github.com:mateors/dailyreport.git 