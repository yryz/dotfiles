![vim-go](https://github.com/yryz/dotfiles/raw/master/screenshots/vim-go.png)

1. **安装 MacVim:**

	`brew install macvim --with-lua`
	
	PS:
	
	>* neocomplete 插件需要`lua`支持
	>* brew 安装macvim需要全功能Xcode，只安装了`Xcode Command Line Tools` 不行，AppStore 下载慢，可以找同事AirDrop共享 `Xcode.app`

2. **.vimrc:**

	```
	cd ~
	git clone https://github.com/yryz/dotfiles
	ln -s dotfiles/vimrc .vimrc
	```

3. **安装vim插件:**
	
	安装vim插件管理器[Vundle](https://github.com/VundleVim/Vundle.vim)  
	`git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim`
	
	`mvim ~/.vimrc` 执行 `:PluginInstall`


4. **安装字体：**

	vimrc中已配置 [Source Code Pro](https://github.com/adobe-fonts/source-code-pro) 字体，[下载字体](https://github.com/adobe-fonts/source-code-pro/archive/2.030R-ro/1.050R-it.zip) 解压后，进入`TTF` 全选所以字体打开，安装字体。
	
5. **配置皮肤：** ([Molokai color scheme for Vim](https://github.com/tomasr/molokai))

	>一键完成
	
	```
	mkdir -p ~/.vim/colors
	curl https://raw.githubusercontent.com/tomasr/molokai/master/colors/molokai.vim > ~/.vim/colors/molokai.vim
	```

6. **vim 插件依赖:**
	>1. **ctrsf.vim插件依赖：** `brew install ack`
	>2. **tagbar插件依赖：** `brew install ctags`
	>3. **vim-go插件依赖：** vim中执行 `:GoInstallBinaries` （自己准备好梯子）
	
7. **MacVim 快捷键冲突映射：**
	系统偏好设置－》键盘－》快捷键－》应用快捷键－》添加，选择`MacVim.app`(brew安装，选择其他，然后`Command+Shift+G`，`/usr/local/Cellar/macvim/` 下面找到):
	
	>- `Command + P` 菜单标题 `Print` 快捷键 `Alt+Command+P`
	>- `Command + F` 菜单标题 `Find...` 快捷键 `Alt+Command+F`
	>- `Command + W` 菜单标题 `Close` 快捷键 `Alt+Command+W`

