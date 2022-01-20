# Annoying .gitignore and friends
The third answer on [this](https://stackoverflow.com/questions/107701/how-can-i-remove-ds-store-files-from-a-git-repository) link is awesome. It has a good list of .gitignores and a global way of setting the config for ez access. For the sake of persistence here is the command to set global git ignores: git config --global core.excludesfile ~/.gitignore_global

And here is the content:

> It is better to copy from this.md file rather than the render for direct copy-pastas.

# Compiled source #
###################
*.com
*.class
*.dll
*.exe
*.o
*.so

# Packages #
############
# it's better to unpack these files and commit the raw source
# git has its own built in compression methods
*.7z
*.dmg
*.gz
*.iso
*.jar
*.rar
*.tar
*.zip

# Logs and databases #
######################
*.log
*.sql
*.sqlite

# OS generated files #
######################
.DS_Store
.DS_Store?
._*
.Spotlight-V100
.Trashes
ehthumbs.db
Thumbs.db
