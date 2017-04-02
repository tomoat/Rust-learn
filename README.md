# Rust Learn

## 安装

在Mac环境下安装（两种方式）

* 通用方式

  > `$ curl https://sh.rustup.rs -sSf | sh`

* brew 方式

  > `brew install rust`

使用通用方式安装完毕之后，需要将 `source $HOME/.cargo/env` 加入到你当前的shell环境中，比如当前为zsh, 就会将此句加入到你的  **~/.zshrc**  文件中。

## 更新

一旦安装完 Rust，更新到最新版本是简单的。在 shell 中运行更新脚本：

> `$ rustup update`

## 卸载

卸载 Rust 同安装一样简单。在 shell 中运行卸载脚本

> `$ rustup self uninstall`

## 验证

安装完 Rust 后，打开 shell，输入：

> `$ rustc —version`

应该能看到类似这样的版本号、提交 hash 和提交日期，对应你安装时的最新稳定版本：

> `rustc x.y.z (abcabcabc yyyy-mm-dd)`

如果出现这些内容，Rust 就安装成功了！

恭喜入坑！（此处应该有掌声！） 

## 本地文档

安装程序也包含一份本地文档的拷贝，你可以离线阅读它们。输入`rustup doc`将在浏览器中打开本地文档。

任何你不太确认标准库中提供的类型或函数是干什么的时候，请查看 API 文档！