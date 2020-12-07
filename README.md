# Rust 生态实践指南 &emsp; [![Build Status travis]][travis]

[Build Status travis]: https://api.travis-ci.com/zzy/rust-crate-guide.svg?branch=master
[travis]: https://travis-ci.com/zzy/rust-crate-guide

Rust 生态实践指南 - The Guide to Rust Crates。

如果欲了解本书，请阅读[本书前言 - https://rust-crate-guide.budshome.com/preface.html](https://rust-crate-guide.budshome.com/preface.html)。

## 在线阅读

《Rust 生态实践指南》，内容规划中。

在线试读地址：[http://rust-crate-guide.budshome.com](http://rust-crate-guide.budshome.com)。

## 离线阅读

如果你喜欢本地阅读方式，可以使用 mdBook（[中文文档](https://mdbook.budshome.com)） 进行书籍构建：

```bash
$ git clone https://github.com/zzy/rust-crate-guide
$ cd rust-crate-guide
$ cargo install mdbook # 指定版本使用参数：--vers "0.3.5"
$ mdbook serve --open # 或者 mdbook build
```

也可以直接用你喜欢的浏览器从 `book` 子目录打开 `index.html` 文件。

```bash
$ xdg-open ./book/index.html # linux
$ start .\book\index.html    # windows
$ open ./book/index.html     # mac
```

## 测试

如果欲运行构建本书的测试组件，请执行：

> 测试组件需要安装一些 crate，中国大陆推荐[更换默认的 Cargo 源为国内镜像源](https://cargo.budshome.com/reference/source-replacement.html)。

```bash
$ cargo test
```

## 贡献

《Rust 生态实践指南》的目的是让 Rust 程序员新手能够更容易地参与到 Rust 语言社区中，因此它需要——并欢迎——你做出自己力所能及的贡献。

### 构建和测试

首先，从 git 克隆《Rust 生态实践指南》并进入目录：

```
git clone https://github.com/zzy/rust-crate-guide.git
cd rust-crate-guide
```

《Rust 生态实践指南》使用 `mdBook`（[中文文档](https://mdbook.budshome.com)）构建，所以需要通过 `Cargo`（[中文文档](https://cargo.budshome.com)）安装它：

```
cargo install --version 0.3.5 mdbook
```

若要在本地生成和阅读《Rust 生态实践指南》，请运行：

```
mdbook serve
```

然后在浏览器中打开 `http://localhost:3000`，即可阅读本书。对源代码所做的任何更改都将自动重新生成页面，并会主动刷新浏览器，因此在编辑源码时打开浏览器窗口是很有帮助的。

书中的所有实例都是使用 [skeptic](https://github.com/brson/rust-skeptic) 测试的，它是测试任意 markdown 文档的工具，风格类似于 rustdoc。

提交前，请对整个仓库进行测试：

```
cargo test
```

祝你学习愉快，欢迎提交问题，欢迎发送 PR。
