# vague-os
[![Build Status](https://travis-ci.com/sn99/vague-os.svg?branch=master)](https://travis-ci.com/sn99/vague-os)

A hobby OS written in Rust

## How to build

2. Install xbuild `cargo install cargo-xbuild`
3. In the vague-os dictionary `rustup override add nightly` followed by `rustup component add rust-src`
4. Build using `cargo xbuild --target x86_64-vague_os.json`
#### Optional steps
5. Download [bootimage](https://github.com/rust-osdev/bootimage) `cargo install bootimage --version "^0.5.0"`
6. Build using bootimage `bootimage build --target x86_64-vague_os.json` to get an ELF file in target/x86_64-vague-os/debug(bootimage.bin) and copy and boot it from a USB or virtual machine
7. Or directly use `bootimage run` is you have [QEMU](https://www.qemu.org/download/) installed

**Basically a dump to everything I learn about OS dev ... a real dump**