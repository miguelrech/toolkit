
File -> Save workspace as ...
   Create folder for workspace like toolkit-projet
File -> Add Folder to workspace
   Create folder inside workspace folder

Example like this:
~/toolkit-project/toolkit   
~/toolkit-project/app

Execute at toolkit:
    go mod init github.com/miguelrech/toolkit
Execute at app
    go mod init application
Execute at ~/toollit-project 
    go work init toolkit app 

Will be created file go.work:

    cat go.work 
    go 1.22.3

    use (
            ./app
            ./toolkit
    )

Execute at toolkit:
git init
