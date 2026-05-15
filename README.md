# AAM (Abstract Alias Mapping)

A robust and lightweight configuration parser `that supports key-value pairs, recursive dependency resolution, file imports, and bidirectional lookups. Designed for applications that need flexible configuration files with references, aliases, and a modular structure.

## Features

- **Simple syntax**: A `key = value` format that is easy to read and write.
- **Import support**: The `@import` directive lets you split configuration into multiple files.
- **Comments support**: Lines starting with `#` are treated as comments.
- **Deep search (`deep_search`)**: Finds all key-value pairs whose key contains a given pattern.
- **Reverse search (`reverse_search`)**: Finds all keys whose value matches a given value.
- **Combined search (`find`)**: First tries a key lookup; if the key does not exist, searches by value.
- **Loop detection**: Safely handles circular dependencies (e.g., `A -> B -> A`) without stack overflows.
- **Config builder (`AAMBuilder`)**: Programmatically generate and save `.aam` files.
- **Typed errors**: Detailed parsing and I/O error handling via `AamlError`.

## Format
You can find documentation and examples for the format in the [docs](https://aam.ininids.in.rs/)
Example:
```aam
# My config
@import base.aam
app_name = rustgames
version = 1.0
```

## Libraries
- [Rust](https://crates.io/crates/aam-rs) (official implementation)
- [Go](https://github.com/ininids/aam-rs) (official Go port)
- [Python](https://pypi.org/project/aam-py/) (official Python port)
- [JavaScript](https://www.npmjs.com/package/aam-js) (official JavaScript port) (Will be published at 2.0.0 version)
- [Java/Kotlin](https://central.sonatype.com/artifact/rs.in.ininids/aam-jv) (official JVM port)
- [C#/.NET](https://www.nuget.org/packages/Aam.Rs/) (official .NET port)
- [Ruby, PHP, WASM, C and others.](https:://github.com/ininids/aam-rs) (Official ports)

### Libraries documentation
- [Rust](https://docs.rs/aam_rs/)
- [README](github.com/INiNiDS/aam-rs?tab=readme-ov-file)

# Coming Soon

- AAM CLI for terminal
- More languages
- AAM v2
- Performance optimizations
- More examples
- New documentation site update