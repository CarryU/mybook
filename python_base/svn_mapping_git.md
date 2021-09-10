|git命令|svn命令|备注|
|--|:--:|--:|
|git --version|svn --version|查看git or svn版本|
|git init|无|不支持，需要服务端操作|
|git clone $url|svn checkout $url 或者svn co $url|下载代码|
|git add|svn add|往版本库中添加新的文件|
|git status|svn status|查看状态|
|git commit -m "$comment"|svn commit -m "$comment"|注：这两个命令是不对等的。git支持本地commit,该提交是提交到了一个缓存区；svn不支持本地commit，commit直接push到远程仓库|
|git push|无|其实git push和svn commit -m "$comment"的功能是一样的，都是把本地代码推送到远程仓库上|
|git pull|svn update 或者 svn up|更新本地的代码与远程仓库代码保持一致|
|git diff|svn diff|比较差异|
|git remote -v|	svn info|查看远程仓库信息|