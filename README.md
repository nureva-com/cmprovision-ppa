# cmprovision-ppa
PPA repository for cmprovision

# Usage

To use this PPA:

```
curl -s --compressed "https://nureva-com.github.io/cmprovision-ppa/KEY.gpg" | gpg --dearmor | sudo tee /usr/share/keyrings/nureva-cmprovision-archive-keyring.gpg
sudo curl -s --compressed -o /etc/apt/sources.list.d/nureva-cmprovision.list "https://nureva-com.github.io/cmprovision-ppa/nureva-cmprovision.list"
sudo apt update
```

# Updating/adding new packages

Put your new .deb files inside the git repo and run `./bin/generate.sh` to
update the files. Then commit and push to repo.
