Required functions for proper submodule management:

git submodule add [submodule-repository-url] 
(make sure your repository has a branch set up)

git submodule add [submodule-repository-url] [path]
if you want to create the submodule in a specific path

git submodule init
The command registers the paths to submodules within the project tree.

git submodule update
The command clones the missing submodules, fetches any new remote commits, and updates the directory tree.
(be careful as this might delete all changes not commited in the submodule)

git submodule foreach '[command]'
The git submodule foreach command allows executing a command on each submodule.
(Use this for commiting changes to all submodules at the same time then you can commit the main
module and you'll have everything up to date)
