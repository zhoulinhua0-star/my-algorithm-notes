## Git workflow

-  在Github上手动创建repo
- 打开Git Bash / Terminal

    ```Bash
    mkdir my-algorithm-notes # 在本地创建新的文件夹
    cd my-algorithm-notes

    git init # 初始化git
    ```

- 将你想复制的项目复制进入新创建的文件夹
- 

    ```Bash
    git status # 检查当前状态

    git add . 
    git commit -m "initial commit: notes and code"
    
    git remote add origin https://github.com/zhoulinhua0-star/my-algorithm-notes # 连接github repo
    git branch -M main # 将当前分支名字改为main
    git push -u origin main
    ```
