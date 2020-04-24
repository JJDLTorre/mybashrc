# mybashrc
Collection of startup scripts I like to have. 

## How to download the .inputrc file
```bash
curl https://raw.githubusercontent.com/JJDLTorre/mybashrc/master/_inputrc -o ~/.inputrc
```

## Mac command prompt
```bash
PS1='\[\e]0;\u@\h \w\a\]\n\[\e[32m\]\u@\h \[\e[33m\]\w\[\e[0m\]\n\$ '
```

## Add up/down arrows to get history matches
Use this on a linux/macOS to allow all users to use up/down arrows to get history commands. 
```
sudo sed -ie 's/^.*: history-search-backward/\"\\e[A\": history-search-backward/' /etc/inputrc
sudo sed -ie 's/^.*: history-search-forward/\"\\e[B\": history-search-forward/' /etc/inputrc
```
