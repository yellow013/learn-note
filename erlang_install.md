- erlang 官网：
http://www.erlang.org


- 安装依赖

yum install gcc glibc-devel make ncurses-devel openssl-devel autoconf

yum install unixODBC unixODBC-devel


- 编译

- 进入解压目录，进行编译

cd otp_src_${version}

./otp_build autoconf

./configure

make

make install



- 配置环境

- erlang 默认安装路径 /usr/local/lib/erlang
- 编辑配置环境变量文件 
vi /etc/profile
- 配置内容如下
export ERLANG_HOME=/usr/local/lib/erlang

export PATH=$ERLANG_HOME/bin:$PATH
- 重新加载配置文件
source /etc/profile
- 查看版本
erl -version
