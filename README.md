# awesome optimizations

## D

- [Improve isAlphaNum](https://github.com/dlang/phobos/pull/8588)
- [Optimize isHexDigit](https://github.com/dlang/phobos/pull/8597)

## Go

- [syscall: use CLONE_VFORK and CLONE_VM](https://github.com/golang/go/commit/9e6b79a5dfb2f6fe4301ced956419a0da83bd025)
- [os, internal/poll, internal/syscall/unix: use copy_file_range on Linux](https://github.com/golang/go/commit/7be3f09deb2dc1d57cfc18b18e12192be3544794)
- [index/suffixarray: index 3-10X faster in half the memory](https://github.com/golang/go/commit/6ca324f2837db696dff8e7d7342280dd5cdf6bca)
- [strconv: use the Eisel-Lemire ParseFloat algorithm](https://github.com/golang/go/commit/a2eb53c571607bb0e64cb2996ca2bd402ad6e347)
- [sort: use pdqsort](https://github.com/golang/go/commit/72e77a7f41bbf45d466119444307fd3ae996e257)
- [hash/crc32: add AMD64 optimized IEEE CRC calculation](https://github.com/golang/go/commit/2027b00e63d9128eaba4a0164072380561c0fc9c)
- [strconv: implement Ryū-like algorithm for fixed precision ftoa](https://github.com/golang/go/commit/0184b445c04a0f30e34ce624298547f12630f3aa)
- [math: amd64 versions of exp and fabs](https://github.com/golang/go/commit/a0117bafa0ddba85a063b958111b1989e39b1a43)
- [sort: use pdqsort](https://github.com/golang/go/commit/72e77a7f41bbf45d466119444307fd3ae996e257)

## Hare

- [strconv: implement Eisel-Lemire fast float parsing algorithm](https://git.sr.ht/~sircmpwn/hare/commit/cc66165dd42e0e89cd641b9fb932b41060580ea7)
- [strconv: implement f32 to string conversion](https://git.sr.ht/~sircmpwn/hare/commit/699fb637b93d19e19cbd97e593fb135685f4406d)

## Java

- [4511638: Double.toString(double) sometimes produces incorrect results](https://github.com/openjdk/jdk/pull/3402)

## Julia

- [Switch float printing from grisu to ryu algorithm](https://github.com/JuliaLang/julia/pull/32799)

## .NET

- [Including FastFloat in parsing process](https://github.com/dotnet/runtime/pull/62301)
- [Adding Int128 and UInt128 with a base software implementation](https://github.com/dotnet/runtime/pull/69204)

## Nim

- [osproc: use clone with CLONE_VM on Linux for faster process spawning](https://github.com/nim-lang/Nim/commit/cd2bd7fa7b1048956c72ad7665b70b2eabecd549)
- [use dragonbox algorithm; alternative to #18008](https://github.com/nim-lang/Nim/pull/18139)

## Python

- [bpo-33671: efficient zero-copy for shutil.copy* functions (Linux, OSX and Win)](https://github.com/python/cpython/pull/7160)
- [bpo-35537: subprocess uses os.posix_spawn in some cases](https://github.com/python/cpython/pull/11452)
- [bpo-35823: subprocess: Use vfork() instead of fork() on Linux when safe](https://github.com/python/cpython/pull/11671)
- [bpo-34561: Switch to Munro & Wild "powersort" merge strategy](https://github.com/python/cpython/pull/28108)
- **WIP** [pycore_condvar.h: remove Windows conditonal variable emulation, use Windows native conditional variable](https://github.com/python/cpython/issues/89464)
  - related: [Issue #15038: Optimize python Locks on Windows](https://github.com/python/cpython/commit/e75ff35af2b6c85d48c68b95f295aeac7396b162)

## Rust

### rust-lang/rust

- [Change Mutex to use SRWLock on Windows](https://github.com/rust-lang/rust/pull/20367)
- [New floating-to-decimal formatting routine](https://github.com/rust-lang/rust/pull/24612)
- [Update substring search to use the Two Way algorithm](https://github.com/rust-lang/rust/pull/26327)
- [Implement a faster sort algorithm](https://github.com/rust-lang/rust/pull/38192)
- [Implement feature sort_unstable](https://github.com/rust-lang/rust/pull/40601)
- [Command: Support posix_spawn() on FreeBSD/OSX/GNU Linux](https://github.com/rust-lang/rust/pull/48624)
- [Support for disabling PLT for better function call performance](https://github.com/rust-lang/rust/pull/54592)
- [Replace HashMap implementation with SwissTable (as an external crate)](https://github.com/rust-lang/rust/pull/58623)
- [specialize io::copy to use copy_file_range, splice or sendfile](https://github.com/rust-lang/rust/pull/75272)
- [Update Rust Float-Parsing Algorithms to use the Eisel-Lemire algorithm](https://github.com/rust-lang/rust/pull/86761)
- [Replace Linux Mutex and Condvar with futex based ones](https://github.com/rust-lang/rust/pull/95035)
- [Introduce deduced parameter attributes, and use them for deducing readonly on indirect immutable freeze by-value function parameters.](https://github.com/rust-lang/rust/pull/103172)
- [x86_64 SSE2 fast-path for str.contains(&str) and short needles](https://github.com/rust-lang/rust/pull/103779)

### rust-lang/compiler-builtins

- [Faster float conversion operations](https://github.com/rust-lang/compiler-builtins/pull/464)

## Swift

- [SwiftDtoa v2: Better, Smaller, Faster floating-point formatting](https://github.com/apple/swift/pull/35299)

## Zig

- [replace quicksort with blocksort](https://github.com/ziglang/zig/commit/75ecfdf66db22942da349d4279b9ddaa8167788f)
- [Parker interface & std.Mutex performance improvements](https://github.com/ziglang/zig/pull/3585)
- [std.Thread.Futex addition](https://github.com/ziglang/zig/pull/9070)
  - and for mutex/condition [std.Thread: Mutex and Condition improvements](https://github.com/ziglang/zig/pull/11497)
- [add new float-parser based on eisel-lemire algorithm](https://github.com/ziglang/zig/pull/11566)
- [partial implementation of printing floating point numbers with errol3](https://github.com/ziglang/zig/commit/7f0620a20fc431717d017d0c19f1e1f29723d93f)
