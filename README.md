# awesome optimizations

## Rust

- [Change Mutex to use SRWLock on Windows](https://github.com/rust-lang/rust/pull/20367)
- [Implement a faster sort algorithm](https://github.com/rust-lang/rust/pull/38192)
- [Implement feature sort_unstable](https://github.com/rust-lang/rust/pull/40601)
- [Command: Support posix_spawn() on FreeBSD/OSX/GNU Linux](https://github.com/rust-lang/rust/pull/48624)
- [Replace HashMap implementation with SwissTable (as an external crate)](https://github.com/rust-lang/rust/pull/58623)
- [specialize io::copy to use copy_file_range, splice or sendfile](https://github.com/rust-lang/rust/pull/75272)
- [Update Rust Float-Parsing Algorithms to use the Eisel-Lemire algorithm](https://github.com/rust-lang/rust/pull/86761)
- [Replace Linux Mutex and Condvar with futex based ones](https://github.com/rust-lang/rust/pull/95035)

## Go

- [syscall: use CLONE_VFORK and CLONE_VM](https://github.com/golang/go/commit/9e6b79a5dfb2f6fe4301ced956419a0da83bd025)
- [index/suffixarray: index 3-10X faster in half the memory](https://github.com/golang/go/commit/6ca324f2837db696dff8e7d7342280dd5cdf6bca)
- [strconv: use the Eisel-Lemire ParseFloat algorithm](https://github.com/golang/go/commit/a2eb53c571607bb0e64cb2996ca2bd402ad6e347)

## Python

- [Switch to Munro & Wild "powersort" merge strategy](https://github.com/python/cpython/pull/28108)
