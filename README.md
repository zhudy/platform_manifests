# platform_manifests
anbox to build android.img

refer: Build Android Image: https://github.com/anbox/anbox/blob/master/docs/build-android.md

$ mkdir $HOME/anbox-work
$ cd $HOME/anbox-work
//GFW workaround: https://mirrors.tuna.tsinghua.edu.cn/help/git-repo/  and https://mirrors.tuna.tsinghua.edu.cn/help/AOSP/
$ curl https://mirrors.tuna.tsinghua.edu.cn/git/git-repo -o repo
$ chmod +x repo
$ sudo mv repo /usr/local/bin/
$sudo ln -s /usr/bin/python3 /usr/local/bin/python //“python”: 没有那个文件或目录

$ export REPO_URL='https://mirrors.tuna.tsinghua.edu.cn/git/git-repo'
$ repo init -u https://github.com/zhudy/platform_manifests/ -b anbox //https://github.com/anbox/platform_manifests.git

$ repo sync -j4
