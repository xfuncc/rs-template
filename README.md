# rs-template

A template for Rust projects.

## Prepare
### Install cargo generate
`cargo generate` 是一个用于生成项目模板的工具。它可以使用已有的 github repository 作为模板生成新的项目。
```bash
cargo install cargo-generate
```
### Install pre-commit
`pre-commit` 是一个用于管理 git hook 的工具。它可以自动运行一些检查，如 `cargo check`、`typos` 等。
```bash
pipx install pre-commit
```
### Install cargo-deny
`cargo-deny` 是一个用于检查 cargo 依赖的工具。它可以检查依赖的安全性、许可证等。
```bash
cargo install --locked cargo-deny
```
### Install typos
`typos` 是一个用于检查拼写错误的工具。
```bash
cargo install typos
```
### Install git-cliff
`git-cliff` 是一个用于生成 changelog 的工具。
```bash
cargo install git-cliff
```
### Install cargo-nextest
`cargo-nextest` 是一个 Rust 增强测试工具。
```bash
cargo install cargo-nextest
```

## Usage

1. 生成项目
```bash
cargo generate --git https://github.com/xfuncc/rs-template
```
2. 修改 `deny.toml` 中的 `db-path` 为你的本地路径。
3. 修改 `cliff.toml` 中的 `<REPO>` 为你的 repository URL。
4. 修改 `Cargo.toml` 中的 `name` 为你的项目名。
5. 修改 `Cargo.toml` 中的 `authors` 为你的名字和邮箱。
6. 修改 `Cargo.toml` 中的 `description` 为你的项目描述。
7. 修改 `Cargo.toml` 中的 `license` 为你的许可证。
8. 运行 `pre-commit install` 安装 git hook。
```bash
pre-commit install
```
