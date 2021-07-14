#### git配置ssh key

cd ~/.ssh // 进入ssh目录
ssh-keygen -t rsa -C "email@mail.com" // 生成rsa密钥
cat .~/ssh/id_rsa_new.pub // 读取生成的公钥，复制添加到github的ssh-key列表中
ssh-add ~/.ssh/id_rsa_new //让ssh识别新的私钥
ssh-add -K KeyPathOrKeyName // 添加到钥匙串
ssh -T git@github.com // 测试是否成功

同一台电脑对应多个GitHub账号的解决方法：https://www.jianshu.com/p/12badb7e6c10





