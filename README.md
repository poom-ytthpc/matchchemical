# matchchemical project

set git .gitconfig

````bash
sm-pull = "! git submodule foreach -q --recursive 'branch=\"$(git config -f $toplevel/.gitmodules submodule.$name.branch)\"; echo $name [$branch] && git checkout $branch && git pull origin $branch'"
````
