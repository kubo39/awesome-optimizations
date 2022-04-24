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
- [os, internal/poll, internal/syscall/unix: use copy_file_range on Linux](https://github.com/golang/go/commit/7be3f09deb2dc1d57cfc18b18e12192be3544794)
- [index/suffixarray: index 3-10X faster in half the memory](https://github.com/golang/go/commit/6ca324f2837db696dff8e7d7342280dd5cdf6bca)
- [strconv: use the Eisel-Lemire ParseFloat algorithm](https://github.com/golang/go/commit/a2eb53c571607bb0e64cb2996ca2bd402ad6e347)
- [sort: use pdqsort](https://github.com/golang/go/commit/72e77a7f41bbf45d466119444307fd3ae996e257)
- [hash/crc32: add AMD64 optimized IEEE CRC calculation](https://github.com/golang/go/commit/2027b00e63d9128eaba4a0164072380561c0fc9c)

## Python

- [bpo-33671: efficient zero-copy for shutil.copy* functions (Linux, OSX and Win)](https://github.com/python/cpython/pull/7160)
- [bpo-35537: subprocess uses os.posix_spawn in some cases](https://github.com/python/cpython/pull/11452)
- [bpo-35823: subprocess: Use vfork() instead of fork() on Linux when safe](https://github.com/python/cpython/pull/11671)
- [bpo-34561: Switch to Munro & Wild "powersort" merge strategy](https://github.com/python/cpython/pull/28108)
- **WIP** [pycore_condvar.h: remove Windows conditonal variable emulation, use Windows native conditional variable](https://github.com/python/cpython/issues/89464)
  - related: [Issue #15038: Optimize python Locks on Windows](https://github.com/python/cpython/commit/e75ff35af2b6c85d48c68b95f295aeac7396b162)

## .NET

- [Including FastFloat in parsing process](https://github.com/dotnet/runtime/pull/62301)
