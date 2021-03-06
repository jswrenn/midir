# midir [![crates.io](https://img.shields.io/crates/v/midir.svg)](https://crates.io/crates/midir) [![Travis Build Status](https://travis-ci.org/Boddlnagg/midir.svg?branch=master)](https://travis-ci.org/Boddlnagg/midir?branch=master) [![AppVeyor Build status](https://ci.appveyor.com/api/projects/status/atit0teb38s2am2y/branch/master?svg=true)](https://ci.appveyor.com/project/Boddlnagg/midir)

Cross-platform, realtime MIDI processing in Rust.

## Features
**midir** is inspired by [RtMidi](https://github.com/thestk/rtmidi) and supports the same features*, including virtual ports (except on Windows) and full SysEx support – but with a rust-y API!

<sup>* With the exception of message queues, but these can be implemented on top of callbacks using e.g. Rust's channels.</sup>

**midir** currently supports the following platforms/backends: 
- [x] ALSA (Linux)
- [x] WinMM (Windows)
- [x] CoreMIDI (macOS, iOS (untested))
- [x] WinRT (Windows 8+), enable the `winrt` feature
- [x] Jack (Linux, macOS), enable the `jack` feature

A higher-level API for parsing and assembling MIDI messages might be added in the future.

## Documentation & Example
API docs can be found at [docs.rs](https://docs.rs/crate/midir/). You can find some examples in the [`examples`](examples/) directory. Or simply run `cargo run --example test_play` after cloning this repository.
