Linux命令
ls:列出文件和目录
ls -l:查看详细信息
ls -lh:可以显示文件大小
ls -a:可以看到隐藏的文件
ls -ld:查看目录的属性
ls -i:查看id号
pwd:显示目前所在位置
mkdir：创建文件夹 例：mkdir a  创建a文件夹
mkdir -p :创建一串目录
touch:创建文件 例：touch a 创建a文件
rm:删除文件
rm -r:删除目录
rm -rf:删除目录（不会进行询问）
rmdir： 删除空白目录
cd ~:进入家目录
cd -:进入上次所在目录
cd ..:进入上一级目录
cp:复制 例如 {cp 文件（或目录）复制到的位置}（如果写一个文件名   相当于更改所复制的文件名字）
cp -r：复制目录
cp -a:复制的时候可以属性一致。
mv:剪切 格式与复制相同（这也是改名的方式，即剪切文件和目标位置   在同一位置）
ln:为文件建立硬链接 格式：ln 文件 目标位置
ln -s:软链接，和快捷方式的功能一样 如果原文件删除 则无法使用
locate:搜索文件，在后台数据库中的文件，但无法搜到新建的文件（    数据库更新是一天左右一更）。
updatedb:手动更新数据库 需要权限
whereis:用来搜索命令所在位置，系统自带命令不能显示
whoami:我是哪个用户
whatis:whatis+命令名 查看命令的功能
which :查看命令别名
find:搜索文件 find [搜索范围](“/”就是根文件) [文件名]  
-exec:衔接两个命令。
grep：搜索字符串 grep [字符串] [文件名] grep -v不包含 grep -i  不区分大小写。
man: 帮助命令 man 1/2/3/4/5/6/7/8 命令 获得不同等级帮助文件 man -f：= whatis 查看命令有哪些帮助等级
man -k:找到该命令的所有帮助信息。
--help:命令操作帮助文档 格式：[命令] --help
zip: 压缩文件 格式：zip [压缩后的文件名] [压缩文件]
zip -r:压缩目录
unzip:解压缩
gzip:压缩文件 格式：gzip [压缩文件] 生成压缩文件后缀名自动  有.gzip 但原文件会消失
gzip -r:压缩目录下的所有文件
ungzip:解压缩=gzip -b 
ungzip -r:解压缩目录下的所有文件
bzip2:压缩文件 不保留源文件
bzip2 -k:压缩文件 保留源文件
bunzip2:解压缩文件
tar -cvf：打包命令 格式：tar -cvf [打包文件名] [源文件]
          -c:打包 -v:显示过程 -f:指定打包后的文件名
tar -jcvf:直接压缩 格式 tar -jcvf [压缩包名.tar.bz2] 源文件
tar -jxvf:解压缩   格式 tar -jxvf [压缩包名.tar.bz2]
shutdown:关机 格式：shutdown [选项] 时间
shutdown -c: 取消关机命令
shutdown -r now:立即重启 可更改now变为指定时间
halt /poweroff /init 0:关机（不安全）
reboot:重启（较为安全） init 6:调用 6级别 （不安全）
logout：退出登录
mount:查看已挂载的目录
挂载命令格式：mount [-t文件系统][-o特殊选项] 设备文件名 挂载点
w：查看登录用户信息
last:查看所有的用户登录信息
lastlog:查看所有用户的最后一次登录
ifconfig:网卡信息
