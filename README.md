# 个人学习记录

立志在本仓库中坚持每日上传学习记录，来勉励自己，目前是一名普通的大二学生，于2025年2月4日开始记录，坚持就是胜利，加油。
将在该仓库中存储学习的代码题目，学习笔记等知识。
主用c语言，python与c++均接触过却未坚持训练，目标将其补回
,将每日复习并训练代码题目，将自己别的知识慢慢积攒起来。

## 仓库知识结构

1. language文件夹下记录c++与python知识笔记
2. note文件夹下
   - xmind文件夹记录思维导图
   - 后续添加
3. code文件夹下
   - c/c++/python记录代码文件
   - 知识笔记用于记录每日题目中学到的知识点
4. eng文件夹下记录每日学习词汇和文章

**每日总结将在README.md文件中**

## 2.4总结

今天终于完成了本地仓库与远程仓库的关联
首先推荐一个git训练项目，网址在https://learngitbranching.js.org/?demo=&locale=zh_CN
明日将该项目复习笔记记录在note中，文件名称git_learn.md

在git remote -v显示结果，配置ssh密钥后，发现git fetch origin出现错误

1. 发现ssh无法连接到github,测试指令`ssh -T  git@github.com`

2. 若发现无效果输入`ssh -T -p 443 git@ssh.github.com`

3. 完成后显示`You've successfully  authenticated,but GitHub does not provide shell access.`

4. 需要启动通过HTTPS的SSH连接
   进入`~/.ssh`目录创建config无后缀文件

   ~~~shell
   Host github.com
   Hostname ssh.github.com
   Port 443
   User git
   ~~~

即可恢复ssh连接