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


# Example outputs

### Using post-merge migration checks
After merging with another branch on Django projects, it's often important to pay attention to migrations. This hook will highlight any migrations that are being merged.

For example:
```

Checking for new migrations we may need to pay attention to...

================================================================================
Please pay special attention to these new migrations: 

codalab/apps/coopetitions/migrations/0001_initial.py
codalab/apps/web/migrations/0040_auto__add_field.py

================================================================================  

```
