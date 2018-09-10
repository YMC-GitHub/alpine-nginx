##### 变量
```
##########
#mongo
##########
# 操作系统
os_type=alpine
os_version=3.8
# 应用环境
app_type=mongodb
app_version=3.2.0

# 用户群组
app_user=mongodb
app_group=mongodb

# 运行依赖
app_run_deps="\
ca-certificates \
curl \
numactl \
"

# 构建依赖
app_build_deps="\
binutils-gold \
curl \
g++ \
gcc \
gnupg \
libgcc \
linux-headers \
make \
python \
"
# 相关目录
app_downlaod_dir=
app_unpack_dir=
app_install_dir=
app_data_dir=/data/db
app_run_dir=/var/run/mongodb/
app_etc_file=/etc/mongod.conf
app_auto_start_file=/etc/init.d/mongod
app_local_time_file=/usr/share/zoneinfo/Asia/Shanghai

##########
#yarn
##########
# 操作系统
os_type=alpine
os_version=3.8
# 应用环境
app_type=yarn
app_version=1.9.4

# 用户群组

# 运行依赖

# 构建依赖
app_build_deps="\
curl gnupg tar\
"
# 相关目录
app_downlaod_dir=
app_unpack_dir=/opt
app_install_dir=/opt
app_link_dir=/usr/local/bin
```

##### 步骤
\# 安装nginx
创连用户和群组
**安装运行时依赖**
安装构建时依赖
下载验证用秘钥
下载软件源码包
验证下载的内容
解压软件源码包
配置编译和安装
删除构建时依赖
删除软件解压包
删除软件源码包

\# 安装yarn
安装构建时依赖
下载验证用秘钥
下载软件安装包
验证下载的来源
建软件安装目录
解压软件安装包
创建软件的软链
移除下载的秘钥
移除软件安装包
移除构建时依赖