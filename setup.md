# Rustチュートリアル セットアップガイド

このガイドでは、Rustプログラミングを始めるために必要な環境構築手順を説明します。

## 1. Rustのインストール

### rustupを使用したインストール（推奨）

rustupはRustの公式インストーラーおよびバージョン管理ツールです。

#### macOS / Linux

ターミナルで以下のコマンドを実行します：

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

#### Windows

[rustup-init.exe](https://win.rustup.rs/)をダウンロードして実行します。

### 環境変数の設定

インストール後、以下のパスを環境変数に追加する必要があります：

```bash
# ~/.bashrc または ~/.zshrc に追加
source $HOME/.cargo/env
```

または、新しいターミナルセッションを開始してください。

## 2. インストールの確認

以下のコマンドでRustが正しくインストールされたか確認します：

```bash
rustc --version
cargo --version
```

以下のような出力が表示されれば成功です：

```
rustc 1.XX.X (xxxxxxxx 20XX-XX-XX)
cargo 1.XX.X (xxxxxxxx 20XX-XX-XX)
```

## 3. 推奨エディタ / IDE

### Visual Studio Code（推奨）

1. [VS Code](https://code.visualstudio.com/)をインストール
2. 拡張機能「rust-analyzer」をインストール

### その他のオプション

- **IntelliJ IDEA** + Rust プラグイン
- **RustRover** (JetBrains製Rust専用IDE)
- **Vim/Neovim** + rust-analyzer

## 4. 最初のプロジェクト作成

新しいRustプロジェクトを作成するには：

```bash
# 新しいプロジェクトを作成
cargo new hello_rust
cd hello_rust

# プロジェクトをビルド
cargo build

# プロジェクトを実行
cargo run
```

「Hello, world!」と表示されれば、環境構築は完了です！

## 5. Rustのアップデート

Rustを最新バージョンにアップデートするには：

```bash
rustup update
```

## 参考リンク

- [The Rust Programming Language (日本語)](https://doc.rust-jp.rs/book-ja/)
- [Rust by Example (日本語)](https://doc.rust-jp.rs/rust-by-example-ja/)
- [Rust 公式サイト](https://www.rust-lang.org/ja)
