## 20220903

### 密码学报模板编译问题

使用texliveonfly无法成功编译，直接使用lualatex可以成功编译，原因未知

## 20220902

### tlmgr安装ctexart

直接`tlmgr install ctexart`是没法安装的，应该将`ctexart`换成`ctex`

### texliveonfly的下载和使用

#### 下载

手动下载的方式比较方便(在ctan中下载)，
因为该包就包含一个说明文件和一个python脚本文件(不用放到指定路径)，
且在archlinux下无法用tlmgr安装(因为texliveonfly需要在root权限下安装，但tlmgr不能在root权限下使用)，

#### 使用

将texliveonfly放入PATH中的任意路径，然后使用命令`texliveonfly <file.tex>`
