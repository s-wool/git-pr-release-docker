# git-pr-release-docker

```
alias git-pr-release='docker run -v $HOME/.ssh:/tmp/.ssh -v $HOME/.gitconfig:/root/.gitconfig -v $SSH_AUTH_SOCK:/ssh-agent -e SSH_AUTH_SOCK=/ssh-agent -v $(pwd):/vol -w /vol -it docker-git-pr-release'
```