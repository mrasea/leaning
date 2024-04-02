# Rust

[官网](https://www.rust-lang.org/)

[rustwiki](https://rustwiki.org/)

## rustup[^1]

[^1]: Rustup：Rust 版本管理器: [https://rustwiki.org/zh-CN/edition-guide/rust-2018/rustup-for-managing-rust-versions.html](https://rustwiki.org/zh-CN/edition-guide/rust-2018/rustup-for-managing-rust-versions.html)

要通过 Rustup 安装 Rust，您可以访问 [安装](https://www.rust-lang.org/install.html)，它将告诉您如何在您的平台上执行此操作。 这将安装 rustup 本身和 `rustc` 和 `cargo` 的 `stable` 版本。

### 安装Rust
安装 Rust 的其他版本，执行 `rustup install`：
```
rustup install 1.30.0
```
对每夜版也是有效的：
```
rustup install nightly-2018-08-01
```
三种最新的版本:
```
$ rustup install stable
$ rustup install beta
$ rustup install nightly
```

### 升级Rust
```
rustup update
```
### 版本管理
设置非 stable 的为默认版本：
```
rustup toolchain default nightly
```
使用一个 toolchain 而不是默认的，`rustup run`：
```
rustup run nightly cargo build
```
还有一个别名，这个更短一些：
```
cargo +nightly build
```
如果您希望每个目录具有不同的默认值，那也很容易！ 如果你在项目中运行它：
```
rustup override set nightly
```
然后当你在那个目录中时，`rustc` 或 `cargo` 的任何调用都将使用该工具链。 要与其他人共享，可以使用工具链的内容创建一个 `rust-toolchain` 文件，并将其检入源代码管理中。 现在，当有人克隆您的项目时，他们将获得正确的版本，而无需自己“覆盖集合”。
