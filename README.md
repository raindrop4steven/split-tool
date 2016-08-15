# 安装步骤

### 1. clone 到本地

```
git clone https://github.com/raindrop4steven/v-vim.git
```


### 2. 安装依赖包


##### 2.1 系统依赖 # ctags, ag(the_silver_searcher)

```
# ubuntu
sudo apt-get install ctags
sudo apt-get install build-essential cmake python-dev  #编译YCM自动补全插件依赖
sudo apt-get install silversearcher-ag

# centos
sudo yum install python-devel.x86_64
sudo yum groupinstall 'Development Tools'
sudo rpm -Uvh http://download.fedoraproject.org/pub/epel/7/x86_64/e/epel-release-7-5.noarch.rpm
sudo yum install the_silver_searcher
sudo yum install cmake

# mac
brew install ctags
brew install the_silver_searcher
```

##### 2.2 使用Python

```
sudo pip install pyflakes
sudo pip install pylint
sudo pip install pep8
```


### 3. 安装

```
进入目录, 执行安装
# 注意原先装过的童鞋, 重装时，不要到~/.vim下执行(这是软连接指向k-vim真是目录)，必须到k-vim原生目录执行
# 会进入安装插件的列表，一安装是从github clone的，完全取决于网速, 之后会自动编译 YCM, 编译失败的话需要手动编译, 有问题见YCM文档
# 如果发现有插件安装失败 可以进入vim, 执行`:PlugInstall'

cd v-vim/
sh -x install.sh
```
