# rsenv
Extra simple companion to https://github.com/semarie/build-rust for easy
switching between Rust versions. Loosely inspired by rbenv.

## Prerequisites
Set `install_dir` in `$HOME/.build_rust.conf`.

## Installation
Prepend this repository `bin/` directory to your `PATH`.

## Usage
```
$ export RSENV_VERSION='nightly'
$ rustc --version
rustc 1.32.0-nightly
$ export RSENV_VERSION='beta'
$ rustc --version
rustc 1.31.0-beta
$ export RSENV_VERSION='system'
$ rustc --version
rustc 1.30.1
$ unset RSENV_VERSION
$ rustc --version
rustc 1.30.1
```

`RSENV_VERSION` can only be `nightly`, `beta` or `system`. If unset or empty, it
defaults to `system`.
