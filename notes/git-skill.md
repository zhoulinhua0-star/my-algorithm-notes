## Git workflow

### 全部流程

```bash
# 1. 创建文件夹
mkdir my-algorithm-notes
cd my-algorithm-notes

# 2. 初始化 git
git init

# 3. 连接远程仓库（先连）
git remote add origin https://github.com/<username>/my-algorithm-notes.git

# 4. 拉取远程（如果是空 repo 可以跳过）
git pull origin main --allow-unrelated-histories --no-edit

# 5. 添加文件
git add .

# 6. 提交
git commit -m "initial commit"

# 7. 推送
git push -u origin main
```