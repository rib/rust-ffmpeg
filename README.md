[![docs.rs](https://docs.rs/ffmpeg-next/badge.svg)](https://docs.rs/ffmpeg-next/)
[![build](https://github.com/rib/rust-ffmpeg/workflows/build/badge.svg)](https://github.com/rib/rust-ffmpeg/actions)

# High-level rust bindings for ffmpeg

This builds on [ffmpeg-sys](https://github.com/rib/rust-ffmpeg-sys) to provide safe, rustic, ffmpeg bindings.

The intention is to reflect the ffmpeg C API as closely as possible so that existing documentation and experience with ffmpeg easily carries over to using this interface.

This repo consolidates work by [meh](https://github.com/meh/rust-ffmpeg) and [zmwangx](https://github.com/zmwangx/rust-ffmpeg)

Currently supported FFmpeg versions: 3.4.x through 4.3.x.

# Documentation:

- [docs.rs](https://docs.rs/ffmpeg-next/);
- [FFmpeg user manual](https://ffmpeg.org/ffmpeg-all.html);
- [FFmpeg Doxygen](https://ffmpeg.org/doxygen/trunk/).

*See [CHANGELOG.md](CHANGELOG.md) for other information on version upgrades.*

A word on versioning: major and minor versions of this crate track major and minor versions of FFmpeg, e.g. 4.2.x of this crate has been updated to support the 4.2.x series of FFmpeg. Patch level is reserved for changes to this crate and does not track FFmpeg patch versions. Since we can only freely bump the patch level, versioning of this crate differs from semver: minor versions may behave like semver major versions and introduce backward-incompatible changes; patch versions may behave like semver minor versions and introduce new APIs. Please peg the version you use accordingly.
