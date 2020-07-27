
1）编译：npm run release


2）提交 ====================================发布git：

# 添加文件
git add .
git commit -m '修改的注释内容'

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