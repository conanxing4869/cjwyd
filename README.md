# 推送代码到 GitHub 操作步骤

## 操作步骤

### 第一步：在 GitHub 新建仓库
1. 打开 https://github.com/new
2. 填写仓库名称（例如 `yd`）
3. 选择 Public 或 Private
4. **不要**勾选 "Initialize this repository with a README"
5. 点击 "Create repository"
6. 复制页面上显示的仓库 URL（格式：`https://github.com/你的用户名/yd.git`）

### 第二步：本地初始化并推送（在终端执行）

```bash
# 进入项目目录
cd C:/Users/83827/Desktop/yd

# 初始化 git 仓库
git init

# 添加所有文件
git add .

# 创建第一次提交
git commit -m "first commit"

# 重命名主分支为 main
git branch -M main

# 添加远程仓库（替换为你的 URL）
git remote add origin https://github.com/你的用户名/yd.git

# 推送到 GitHub
git push -u origin main
```

### 第三步：身份验证
- 推送时 GitHub 会要求登录
- 推荐使用 **Personal Access Token (PAT)** 作为密码
  - 生成地址：GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
  - 权限勾选：`repo`ajshaidhqu
