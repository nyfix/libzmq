This is the NYFIX version of libzmq (https://github.com/zeromq/libzmq).




Steps to create
---

First setup an empty repo in gitlab.
    
```
git clone http://gitlab.ullink.lan/wtorpey/libzmq.git
git commit --allow-empty -n -m "Initial commit" .
git push origin master
git subtree add --prefix=upstream --squash https://github.com/zeromq/libzmq.git master
git commit -m "Add upstream subtree for libzmq"
git push origin master
```    

Note that the initial (empty) commit and push are needed to avoid the error: "fatal: ambiguous argument 'HEAD': unknown revision or path not in the working tree."

