# git-save-life
## Corrigir mensagem com erro
<code>git commit -m "new message" --amend</code>

## 
*Cuidado perde todas as modificações*  
<code>git reset --hard</code>  
Volta o commit mais mantem as modficações   
<code>git reset --soft</code>  

*Reseta a branch co base no remote*
<code>git fetch origin
git reset --hard origin/master
</code>
https://stackoverflow.com/questions/1628088/reset-local-repository-branch-to-be-just-like-remote-repository-head

[Push Branch to Another Branch](https://devconnected.com/how-to-push-git-branch-to-remote/#:~:text=In%20order%20to%20push%20your,name%20of%20the%20remote%20branch.)

<code>git push < remote> <local_branch>:<remote_name> </code>

## Resolver conflito ao dar o pull
O seus commits virao na frente nao alterando a ordem que esta no repositorio  
<code>git pull --rebase</code>  
<img src="imagens/rebase" style="width:400px;height:150px;"></img>  
Caso der conflito, resolver e adicionar as alteracoes.  
<code>git pull rebase --continue</code>  



## Adicionar origin 
[help1](https://stackoverflow.com/questions/42830557/git-remote-add-origin-vs-remote-set-url-origin)

[help2](https://docs.github.com/pt/get-started/getting-started-with-git/managing-remote-repositories)

below is used to add a new remote:  
<code>git remote add origin git@github.com:User/UserRepo.git<code>  

below is used to change the url of an existing remote repository:  
<code>git remote set-url origin git@github.com:User/UserRepo.git<code>  

below will push your code to the master branch of the remote repository defined with origin and -u let you point your current local branch to the remote master branch:
<code>git push -u origin master<code>
