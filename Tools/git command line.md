#### git配置ssh key

cd ~/.ssh // 进入ssh目录
ssh-keygen -t rsa -C "email@mail.com" // 生成rsa密钥
cat .~/ssh/id_rsa_new.pub // 读取生成的公钥，复制添加到github的ssh-key列表中
ssh-add ~/.ssh/id_rsa_new //让ssh识别新的私钥
ssh-add -K KeyPathOrKeyName // 添加到钥匙串
ssh -T git@github.com // 测试是否成功

同一台电脑对应多个GitHub账号的解决方法：https://www.jianshu.com/p/12badb7e6c10
思路是在.ssh/config文件中添加多个Host与IdentifyFile的对照：

```shell
  #Default GitHub
  Host github.com
  HostName github.com
  User git
  IdentityFile ~/.ssh/id_rsa

  Host github-personal
  HostName github.com
  User git
  IdentityFile ~/.ssh/id_rsa_personal
```

#### git仓库设置

git config --list // 查看git配置
git config --global user.name "userName" // 全局配置
git config --global user.email "xxx@xx.com"
git config user.name "userName" // 只配置当前项目
git config user.email "xxx@xx.com"

git remote -v // 查看远程仓库地址
git remote set-url origin https://github.com/user/repo2.git // 修改远程仓库地址，可切换shh、http







