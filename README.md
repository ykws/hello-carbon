# Hello, Carbon

[![macOS](https://img.shields.io/badge/macOS-Monterey-black)](https://developer.apple.com/macos/)

## The Article

It had attracted me about Carbon.

> If Rust works for you today, you should use it. But moving a C++ ecosystem to Rust is hard.

https://9to5google.com/2022/07/19/carbon-programming-language-google-cpp/

## Getting started

```
# Install bazelisk using Homebrew
$ brew install bazelisk

# Install Clang/LLVM using Homebrew
$ brew install llvm
$ export PATH="${PATH}:$(brew --prefix llvm)/bin"
$ export LDFLAGS="-L$(brew --prefix llvm)/lib"
$ export CPPFLAGS="-I$(brew --prefix llvm)/inclue"

# Check export
$ tail -3 /.zshrc
export PATH=$PATH:/opt/homebrew/opt/llvm/bin
export LDFLAGS="-L/opt/homebrew/opt/llvm/lib"
export CPPFLAGS="-I/opt/homebrew/opt/llvm/include"

# Download Carbon's code.
$ git clone git@github.com:carbon-language/carbon-lang.git
$ cd carbon-lang

# Build and rub the explorer.
$ bazel run //explorer -- ./explorer/testdata/print/format_only.carbon
```

https://github.com/carbon-language/carbon-lang/blob/trunk/README.md#getting-started

