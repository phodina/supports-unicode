Detects whether a terminal supports unicode.

This crate is a Rust port mashing together
[@sindresorhus](https://github.com/sindresorhus)'
[`is-unicode-supported`](https://npm.im/is-unicode-supported) and
[@iarna](https://github.com/iarna)'s
[`has-unicode`](https://npm.im/has-unicode) NPM packages.

> Rust >= 1.54 is needed to build this project (supports invoking function-like
> macros inside attributes)

## Example

```rust
use supports_unicode::Stream;

if supports_unicode::on(Stream::Stdout) {
    println!("stdout supports unicode output");
} else {
    println!("no unicode, please");
}
```
