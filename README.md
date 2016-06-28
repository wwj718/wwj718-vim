# wwj718-vim
my vimrc

# Usage
### 不使用插件
wget https://raw.githubusercontent.com/wwj718/wwj718-vim/master/wwj718_vim_vimrc -O ~/.vimrc

然后注释掉

```
" install bundles
if filereadable(expand("~/.vimrc.bundles"))
  source ~/.vimrc.bundles
endif
```

### 使用插件
*  git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
*  wget https://raw.githubusercontent.com/wwj718/wwj718-vim/master/wwj718_vim_vimrc -O ~/.vimrc
*  wget https://raw.githubusercontent.com/wwj718/wwj718-vim/master/wwj718_vim_vimrc_bundles -O ~/.vimrc.bundles
*  vim +PluginInstall +qall


# 说明
以上配置对vim和macvim同时有效

### neovim
wget https://raw.githubusercontent.com/wwj718/wwj718-vim/master/wwj718_vim_vimrc -O ~/.config/nvim/init.vim

注释掉插件部分
```
" install bundles
if filereadable(expand("~/.vimrc.bundles"))
  source ~/.vimrc.bundles
endif
```

neovim插件安装：

*  curl -fLo ~/.config/nvim/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
*  在 ~/.config/nvim/init.vim添加你要的插件

```
call plug#begin('~/.vim/plugged')
Plug 'scrooloose/nerdtree', { 'on':  'NERDTreeToggle' }
map <F7> :NERDTreeToggle<CR>
call plug#end()
```



