# Zero To Production In Rust

<div align="center"><a href="https://zero2prod.com" target="_blank"><img src="https://www.zero2prod.com/assets/img/zero2prod.png" width="75%" /></a></div>

[Zero To Production In Rust](https://zero2prod.com) is an opinionated introduction to backend development using Rust, where project based learing is employed using a email newsletter server as the motivating example.

This is a personal repository used for working through the book.

## Pre-requisites

You'll need to install:

- [Rust](https://www.rust-lang.org/tools/install)
- [Docker](https://docs.docker.com/get-docker/)

There are also some OS-specific requirements.

### Windows
  
```bash
cargo install -f cargo-binutils
rustup component add llvm-tools-preview
```

### Linux

```bash
# Ubuntu 
sudo apt-get install lld clang
# Arch 
sudo pacman -S lld clang
```

### MacOS

```bash
brew install michaeleisel/zld/zld
```

## How to build

Launch a (migrated) Postgres database via Docker:

```bash
./scripts/init_db.sh
```

Launch `cargo`:

```bash
cargo build
```

## How to test

Launch a (migrated) Postgres database via Docker:

```bash
./scripts/init_db.sh
```

Launch `cargo`:

```bash
cargo test 
```
