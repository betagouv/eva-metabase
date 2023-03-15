This dépot is the eva fork of the official metabase depot from scalingo.

[original README](original_readme.md)

## Configuration
```bash
$ scalingo --app eva-metabase git-setup
$ git remote rename scalingo deploy
$ git remote add scalingo_origin git@github.com:Scalingo/metabase-scalingo.git
```

## To update metabase

simply re-push to `deploy` remote, using -f

## Deploying after updating from original scalingo depot

```bash
$ git pull scalingo_origin --rebase=false master
$ git push deploy master
$ git push
```
