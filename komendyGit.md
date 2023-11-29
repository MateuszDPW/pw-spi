# git

## git init

Opis: Inicjalizuje nowe repozytorium Git.
Przykład:

git init

## git clone

Opis: klonuje istniejące repo z podanego URL.
Przykład:

git clone https://github.com/user/repo.git

git clone [url] [katalog] /

git clone [url] [katalog] ~

git clone --branch [branch-name] [url]

git clone --depth 1 [url]

git clone --mirror [url]

## git add

git add [file]
git add [directory]
git add . git add -A
git add -u
git add --ignore-removal
git add [file1] [file2]
git add "*.py"

## git commit

git commit -m "[commit message]"
git commit -a -m "[commit message]"
git commit --amend -m "[change last commit message]"
git commit --amend --no-edit
git commit --allow-empty -m "Pusty commit"
git commit -m "Tytuł commita" -m "Dalszy opis zmian"

## git status

git status 
git status -s
git status -u
git status -b
git status --show-stash

## git pull

git pull
git pull origin
git pull origin dev
git pull --verbose
git pull --dry-run
git pull --no-commit origin feature

## git remote

git remote
git remote -v
git remote add [nazwa] [URL]
git remote -rm [nazwa]
git remote --rename <stara nazwa> <nowa nazwa>
git remote show [shortname]
git remote update
git remote set-url [nazwa] [nowy-url]
git remote set-head [nazwa] -a

## git push

git push

## git config

git config --global user.name "[nazwa]"
git config --global user.email "[email]"
git config --local user.name "[nazwa]"
git config --local user.email "[email]"
git config --global core.editor "[editor]"
git config --list
git config user.email
git config --global alias.[alias-name] '[command]'
git config --global alias.st 'status'
git config --global core.autocrlf [true|false|input]
git config --global core.ignorecase [true|false]
git config --global merge.tool [tool]
git config --global diff.tool [tool]
git config --global core.filemode [true|false]

## rebase vs merge

## git branch

git branch
git branch [nazwa]
git branch -d [nazwa]
git branch -D [nazwa]
git branch -m [old-name] [new-name]
git branch -r
git branch -a
git branch --show-current
git branch -v
git branch --no-merged [branch]
git branch --merged [branch]
git branch --contains [commit]
git branch -vv
git branch --sort=[key]
git branch --sort=committerdate
git branch [branch-name] [start-point]
git branch --copy [feature-old] [feature-new]
git branch --move [old-branch] [new-branch]
git branch --edit-description [branch-name]
git branch --list [pattern]
git branch --list 'feature*'
git branch --delete --remotes [remote/branch] (usuwanie zdalnego repo)
git branch --force [branch-name]

## git checkout

git checkout [branch-name]
git checkout -
git checkout -b [branch-name]
git checkout [commit-hash]
git checkout -- [file-name]
git checkout [branch-name] 
git checkout --orphan new-start
git checkout [tag-name]
git checkout v1.0.0
git checkout -b [new-branch] [start-point]

## git tag

git tag [tag-name]
git tag -a [tag-name] -m "[message]"
git tag -d [tag-name]
git show [tag-name]
git push [remote] [tag-name]
git tag -l [pattern]
git tag -l "v1"
git tag -a [tag-name] [commit-hash] -m "[message]"

## git reset

git reset
git reset [file]
git reset --soft [commit]
git reset --soft HEAD~1
git reset --hard [commit]
git reset --keep [commit]



