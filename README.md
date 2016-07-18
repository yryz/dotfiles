![vim-go](https://github.com/yryz/dotfiles/raw/master/screenshots/vim-go.png)

**安装 MacVim:**

`brew install macvim --with-lua`

neocomplete 插件需要lua支持

**.vimrc:**

```
cd ~
git clone https://github.com/yryz/dotfiles
ln -s dotfiles/vimrc .vimrc

```

**安装vim插件:**

[安装vim插件管理器Vundle](https://github.com/VundleVim/Vundle.vim)

`mvim ~/.vimrc` 执行 `:PluginInstall`


**安装字体：**

[Source Code Pro](https://github.com/adobe-fonts/source-code-pro)

**配置皮肤：**
[Molokai color scheme for Vim](https://github.com/tomasr/molokai)

`mkdir -p ~/.vim/colors`
`curl https://raw.githubusercontent.com/tomasr/molokai/master/colors/molokai.vim > ~/.vim/colors/molokai.vim`

**MacVim 快捷键冲突映射：**
系统偏好设置－》键盘－》快捷键－》应用快捷键－》添加，选择MacVim.app:

- `Command + P` 菜单标题 `Print` 快捷键 `Alt+Command+P`
- `Command + F` 菜单标题 `Find...` 快捷键 `Alt+Command+F`
- `Command + W` 菜单标题 `Close` 快捷键 `Alt+Command+W`

---
**ctrsf.vim插件依赖：** 
`brew install ack`

**tagbar插件依赖：** 
`brew install ctags`

**vim-go插件依赖：**
vim中执行 `:GoInstallBinaries` （自己准备好梯子）

