# Workflow
> 迭代 + 上线流程的闭环


## 新迭代
1. 从master 拉取新的分支，如（dev_1.0.7）
2. 切换到dev_1.0.7分支
3. 在docs目录下，建立新的dev_1.0.7.md的release notes文件
4. 开始第一次提交


## 上线封包 tag
1. 测试同学确认没有问题之后，运行相应的命令如：weipai prd 1.0.7 打好生产包
2. 邮件通知运维同学，上线
3. 上线后，测试同学测试，如果有紧急问题，可提新的版本如： dev1.0.7.1 修复紧急bug(流程参考：新迭代)
4. 封包，合代码到master： 如果上述流程没有问题，上线稳定之后，就可以合并代码到master分支
5. 打tag: 封包之后，打tag ，命名：v1.0.7 (这个版本号与dev的完全一致)
