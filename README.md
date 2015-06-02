# git-hooks
My personal git hooks I use on most projects (relevant to django, python, web dev)


# Installing

### Per-project

Edit ```.git/hooks/<hook>``` where `<hook>` can be something like `post-merge`

### Globally

Create the git template
```$ git config --global init.templatedir '~/.git_templates'```

Create the folder
```$ mkdir ~/.git_templates```

Insert whatever hooks you want like ```hooks/post-merge```, `chmod +x` them

Go to your git repo and `git init` to pull down the hooks

