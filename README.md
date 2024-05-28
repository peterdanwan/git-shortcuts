# ⏩ git-shortcuts ⏩

## How to use

1. Have `Git` [installed](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).
2. Copy, paste, and enter the command below to add one of these pre-defined git aliases:

   ```sh
   git config --global alias.GIT_SHORTCUT "EVALUATES_TO"
   ```

   - NOTE: replace `GIT_SHORTCUT` with a git shortcut and `EVALUATES_TO` to what the shortcut will evaluate to

### Example

```sh
git config --global alias.cm "commit -m"
```

- Now, when do make your next commit, you can use `git cm "concise message of what was changed"` instead of `git commit -m "concise message of what was changed"`.

## Aliases

| git shortcut         | Evaluates to                                         | What it does                                                                                                           |
| -------------------- | ---------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| `a`                  | add                                                  | Allows you to use `add` to add file(s) to your staging area                                                            |
| `cm`                 | commit -m                                            | Shortcut to writing the verbiage needed before writing a commit message                                                |
| `co`                 | checkout                                             | Allows you to use checkout                                                                                             |
| `d`                  | diff                                                 | Allows you to use diff                                                                                                 |
| `get-alias`          | !f() { git config --get alias.$1; }; f               | Shows what a given git alias evaluates to                                                                              |
| `get-aliases`        | !git config --get-regexp alias \| sort               | Shows your git aliases (sorted alphabetically), and what they evaluate to                                              |
| `get-aliases-origin` | !git config --get-regexp --show-origin alias \| sort | Shows your git aliases (sorted alphabetically), what they evaluate to and where they're stored (local, global, system) |
| `rao`                | remote add origin                                    | Allows you to quickly add your remote repository to your local repository, naming it `origin`                          |
| `lag`                | log --all --graph                                    | Shows all the repo's commit history and any different branches it has                                                  |
| `rm-alias`           | !f() { git config --global --unset alias.$1; }; f    | Removes a singular global alias                                                                                        |
| `s`                  | status                                               | Allows you to use status                                                                                               |
| `ss`                 | status -s                                            | Allows you to use status with the -s modifier to see the status of your files (not which branch you're on)             |
