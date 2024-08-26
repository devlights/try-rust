# try-rust

This is my TUTORIAL project for rust.

[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/devlights/try-rust)

## Run

```sh
$ task -d /path/to/example
```

```sh
$ task -d helloworld/
task: [default] cargo run
   Compiling helloworld v0.1.0 (/home/dev/dev/github/try-rust/helloworld)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.24s
     Running `/home/dev/dev/github/try-rust/target/debug/helloworld`
[00] Hello, world!
[01] Hello, world!
[02] Hello, world!
```

## サンプルの追加方法

1. Cargo.toml に プロジェクト名 を追加

```toml
[workspace]
resolver = "2"
members = [
    "helloworld",
]
```

2. cargo new でプロジェクトを追加

```sh
$ cargo new name-of-project
```

## REFERENCES

- Tour of Rust
  - https://tourofrust.com/00_ja.html
- The Rust Programming Language 日本語版
  - https://doc.rust-jp.rs/book-ja/
- １つのgitリポジトリにcargoのワークスペースを複数作成する
  - https://zenn.dev/shotaro_tsuji/articles/583bd9dc8dc12f
- RustでCargoの仮想ワークスペース（virtual workspaces）使用時にのみ依存パッケージのコンパイルに失敗する
  - https://blog.publictheta.com/memos/aGNz9GK17bQnR04Ee4ySd
