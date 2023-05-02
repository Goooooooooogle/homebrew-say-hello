## 本地通过brew安装
#### 1. 生成可执行程序，发布到GitHub
例如: [Goooooooooogle/say-hello](https://github.com/Goooooooooogle/say-hello/releases/tag/v0.0.1)
#### 2. 生成一个formula

`brew create --tap Goooooooooogle/homebrew-say-hello https://github.com/Goooooooooogle/say-hello/releases/download/v0.0.1/say-hello`
> `--tap` Generate the new formula within the given tap, specified as user/repo.  
> 生成的文件位置: `/opt/homebrew/Library/Taps/goooooooooogle/homebrew-say-hello`
#### 3. 此时可以通过命令安装
`brew install say-hello`

## 发布程序到homebrew
#### 1. 新建一个GitHub仓库 `Goooooooooogle/homebrew-say-hello`, 需要以 `homebrew-` 开头
#### 2. 把上一步生成的formula文件放到新建的仓库里
#### 3. 安装homebrew的tap `brew tap Goooooooooogle/homebrew-say-hello`
#### 4. 此时可以直接安装命令 `brew install say-hello`
