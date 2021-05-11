### neovim 的 golang 开发环境配置



##### 1. neovim



旧版本 neovim 不支持 vim-go 插件，从 Github 下载新版本的 neovim

https://github.com/neovim/neovim/releases



下载 nvim-linux64.tar.gz 文件，解压缩：

```shell
tar -zxvf nvim-linux64.tar.gz
```



在 .bashrc（或其他可用的启动文件） 添加命令别名：

```shell
alias vim = '<path-to-nvim>/bin/nvim'
```



##### 2. vim-plug



```shell
curl -fLo ~/.config/nvim/autoload/plug.vim --create-dirs \ https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```



##### 3. 编辑 ~/.config/nvim/init.vim 文件

随后 `vim` 打开编辑器，下载插件 `:PlugInstall`。
