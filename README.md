# async-task

[![Build Status](https://travis-ci.com/async-rs/async-task.svg?branch=master)](https://travis-ci.com/async-rs/async-task)
[![License](https://img.shields.io/badge/license-MIT%2FApache--2.0-blue.svg)](
https://github.com/async-rs/async-task)
[![Cargo](https://img.shields.io/crates/v/async-task.svg)](https://crates.io/crates/async-task)
[![Documentation](https://docs.rs/async-task/badge.svg)](https://docs.rs/async-task)
[![chat](https://img.shields.io/discord/598880689856970762.svg?logo=discord)](https://discord.gg/JvZeVNe)

Task abstraction for building executors.

To spawn a future onto an executor, we first need to allocate it on the heap and keep some
state alongside it. The state indicates whether the future is ready for polling, waiting to be
woken up, or completed. Such a future is called a *task*.

This crate helps with task allocation and polling its future to completion.

## License

Licensed under either of

 * Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.

#### Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be
dual licensed as above, without any additional terms or conditions.
