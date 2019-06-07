### web
- 1.javascript vue.js html template

### command 
- 1.执行cnpm install vue-cli -g 全局安装
- 2.vue init webpack "名称" eg: vue init webpack vue-name
- 3.npm install 安装依赖库
- 4.npm install vue axios bootstrap
- 5.npm run dev 启动项目

### npm init 

### npm install vue axios bootstrap

## git rebase操作步驟記錄
```
. 想获取develop的最新版本必须先切换到develop  --------git checkout develop
. git pull origin develop  获取最新的develop版本
. 需要先切换到自己的分支，才能对develop进行rebase -----git checkout NewFix
. git rebase develop  把自己新开发的功能快进最新版本
. 这时候需要先切换到主干才能把自己的分支合并  ------git checkout develop
. git merge NewFix  这时候才能合并
. git push origin develop  推到自己的起源代码仓库
. 在网页上创建pull request向管理员提交变更
```

### git rabase 用法
```
git pull --rebase origin master  
```
OR 
```
git fetch origin
git rebase origin/master
```

### 远程登录SSH免密
- 生成公私钥 ssh-keygen -t rsa
- 将公钥上传到目标服务器 ssh-copy-id -i ~/.ssh/id_rsa.pub username@ip
