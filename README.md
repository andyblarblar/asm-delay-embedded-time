This is a fork of asm-delay that uses embedded-time traits instead of the otherwise uncommon bitrate crate.

# `asm-delay-embedded-time`

> no_std implementation of embedded-hal's DelayMs & DelayUs for cortex-m.


## Basic usage

Include [library](https://crates.io/crates/asm-delay-embedded-time) as a dependency in your Cargo.toml
[![crates.io](http://meritbadge.herokuapp.com/asm-delay?style=flat-square)](https://crates.io/crates/asm-delay-embedded-time):

```
[dependencies.asm-delay-embedded-time]
version = "<version>"
```

```rust
use embedded_hal::prelude::*;
use asm_delay_embedded_time::AsmDelay;
use asm_delay_embedded_time::embedded_time::rate::*;

let d = AsmDelay::new(64.MHz());
d.delay_ms(5);
```

## Documentation

API Docs available on [docs.rs](https://docs.rs/asm-delay-embedded-time).

## License

Licensed under

- MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)
