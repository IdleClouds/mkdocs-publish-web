# 使用技巧

1、层级可通过多个#区分，共6层<br/>

```bash
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

2、折叠块

```bash
<details>
<summary>点击展开详情</summary>
内容写在这里
</details>
```
3、图片

(1)、语法
```bash
![图片描述文字](图片相对路径 "鼠标悬浮提示文字")
```
(2)、文件夹结构
```bash
docs/
├── github.md
├── quickstart.md
└── assets/        # 统一存放所有图片资源
    ├── github/    # github.md专属配图
    └── common/    # 全局公用截图
```
（3）、图片命名
```bash
1、全部小写
2、单词用短横线-分割
3、格式：模块-用途-序号.png
4、后缀统一：优先png(截图)，jpg(照片)
```

4、发布
```bash
先提交md源码到main/master分支
1、git add .
2、git commit -m "docs:更新文档内容"
3、git push origin main
再执行部署命令
4、mkdocs gh-deploy --clean
```


