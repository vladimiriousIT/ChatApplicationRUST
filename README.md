![RUST](https://en.wikipedia.org/wiki/Rust_(programming_language)#/media/File:Rust_programming_language_black_logo.svg)
========
# Chat Application with RUST
Chat Application with RUST Client/Server Side in the repo :)

This is the main source code repository for [Rust]. It contains the compiler,
standard library, and documentation.

[Rust]: https://www.rust-lang.org

## Quick Start
[quick-start]: #quick-start

Read ["Installation"] from [The Book].

["Installation"]: https://doc.rust-lang.org/book/second-edition/ch01-01-installation.html
[The Book]: https://doc.rust-lang.org/book/index.html

## Building from Source
[building-from-source]: #building-from-source

### Building on *nix
1. Make sure you have installed the dependencies:

   * `g++` 4.7 or later or `clang++` 3.x or later
   * `python` 2.7 (but not 3.x)
   * GNU `make` 3.81 or later
   * `cmake` 3.4.3 or later
   * `curl`
   * `git`

2. Clone the [source] with `git`:

   ```sh
   $ git clone https://github.com/rust-lang/rust.git
   $ cd rust
   ```

[source]: https://github.com/rust-lang/rust

3. Build and install:

    ```sh
    $ git submodule update --init --recursive --progress
    $ ./x.py build && sudo ./x.py install
    ```

    > ***Note:*** Install locations can be adjusted by copying the config file
    > from `./config.toml.example` to `./config.toml`, and
    > adjusting the `prefix` option under `[install]`. Various other options, such
    > as enabling debug information, are also supported, and are documented in
    > the config file.

    When complete, `sudo ./x.py install` will place several programs into
    `/usr/local/bin`: `rustc`, the Rust compiler, and `rustdoc`, the
    API-documentation tool. This install does not include [Cargo],
    Rust's package manager, which you may also want to build.

[Cargo]: https://github.com/rust-lang/cargo

### Building on Windows
[building-on-windows]: #building-on-windows

There are two prominent ABIs in use on Windows: the native (MSVC) ABI used by
Visual Studio, and the GNU ABI used by the GCC toolchain. Which version of Rust
you need depends largely on what C/C++ libraries you want to interoperate with:
for interop with software produced by Visual Studio use the MSVC build of Rust;
for interop with GNU software built using the MinGW/MSYS2 toolchain use the GNU
build.
