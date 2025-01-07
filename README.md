# pages
static_pages

```
# 重建
cd /Users/infra02/MEGAsync/github.com
_date=`date '+%Y%m%d-%H%M%S'`
mv openvpn-new openvpn-new-${_date}
git clone --branch main https://github.com/agent7-cloud/pages.git

# 更新
_date=`date '+%Y%m%d-%H%M%S'`
cd ~/Users/infra02/MEGAsync/github.com/pages
_date=`date '+%Y%m%d-%H%M%S'`
git add .
git commit -m "add ${_date}"
git push -u origin main
```

```
# 列出本地分支
git branch

# 列出所有分支（包含遠端分支）
git branch -a

# 拉取遠端分支
git fetch origin

# 拉取遠端分支並切換
git fetch origin
git checkout -b 本地分支名稱 origin/遠端分支名稱

# 切換到 己存在分支
git checkout 分支名稱
```
