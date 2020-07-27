
1）编译：npm run release


2）提交 ====================================发布git：

# 【Commit规范- Type】
# feat：新功能（feature）
# fix：修补bug
# docs：文档（documentation）
# style： 格式（不影响代码运行的变动）
# refactor：重构（即不是新增功能，也不是修改bug的代码变动）
# test：增加测试
# chore：构建过程或辅助工具的变动


# 第一次
# git add .

# 有修改项
# 添加文件（注意修饰fix，冒号后面有个空格） 
git commit -m 'feat: 新功能的注释内容'
git commit -m 'fix: 修补bug的注释内容'

# 千万注意，-a不会造成新文件被提交，只能修改。
git commit -a -m "Changed some files"

# 提交到远程仓库by tag
git push --follow-tags origin master 


3）发布 =========发布到npm
npm adduser

# 发布到（@jefth/tinyapi）：
npm publish --access public



////////////////////////////////////////////////////
无法发布到私有包
这个当你的包名为@your-name/your-package时才会出现，
原因是当包名以@your-name开头时，npm publish会默认发布为私有包，但是 npm 的私有包需要付费，所以需要添加如下参数进行发布:

npm publish --access public
原文链接 链接：https://www.jianshu.com/p/40f732d91a8c


//////////////git commit 规范不对导致报错
https://blog.csdn.net/yutingwu816/article/details/104391678?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-3.edu_weight&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-3.edu_weight


