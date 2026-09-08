# 使用技巧
1、仓库命名规范
````bash
1、全部小写
2、单词分隔用-
3、区分类型：业务项目/组件库/工具脚本/文档/Demo
分隔符统一规则：仓库名= - ；分支名= / ；tag版本号= v主.次.修订
````
2、通过git上传源码到仓库
````bash
第一次上传：
1、新建.gitignore文件，记录不需要上传的文件夹或者类型文件
2、git init    #初始化本地git仓库，项目根目录下下生成.git文件夹
3、git add .   #扫描整个项目除了忽略的文件，把剩余加入暂存区
4、git commit -m "备注内容"   #把暂存区的文件保存成一次本地版本快照，存在.git仓库里
5、git remote add origin https://github.com/用户名/仓库名.git  #绑定远程仓库地址
6、git push -u origin master或者main

后续更新：
1、git add .
2、git commit -m "更新内容"
3、git push

备注:
1、git branch -M main #修改本地master名字为main

````


