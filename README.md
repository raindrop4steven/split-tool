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
cd v-vim/ && sh -x install.sh
```
