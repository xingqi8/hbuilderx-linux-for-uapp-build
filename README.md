# hbuilderx-linux-for-uapp-build
互联网收集的HbuildX Linux环境下通过uapp打包发布uniapp的依赖程序，可以用作Linux环境下的Devops CI CD.

Linux环境：
node 版本必须为 v16，保证和 hbx 内置 node 版本一致。
uapp 版本 >= 2.3.5
uapp  -v 可以查看当前使用版本


使用：
1、下载hbuilderx-linux-3.98.tar.gz 传到 linux 服务器下，解压到 /usr/local/ 目录下，解压后的目录为：/usr/local/hbuilderx-linux
2、配置node 和 hbx 环境变量
npm install -g uapp
uapp sdk init           # 初始化或更新 uappsdk
uapp config hbx.dir /usr/local/hbuilderx-linux
uapp config node `which node`
3、编译
uapp run build:h5
uapp run build:mp-weixin
更多使用详细可参考uapp仓库
uapp github地址：https://github.com/uappkit/uapp
