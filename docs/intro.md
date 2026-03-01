---
sidebar_position: 1
title: "Introduction"
---

# AAM (Abstract Alias Mapping)
## Introducing AAM
Configuration files have a tendency to grow uncontrollably. They become bloated, difficult to read, and even harder to maintain. Splitting them into multiple files helps, but it doesn't solve the underlying complexity of managing data relationships. We needed a more intuitive way to handle mappings — we needed AAM.
### The problem - Verbose Mapping
Imagine you need to manage a large set of bidirectional aliases (where you can look up a key by value and vice-versa). In formats like TOML, you're forced into boilerplate:
```toml
[alias]
a = "b"
b = "a"
```
That's three lines for a single mapping. Multiply that by a hundred, and your config becomes a nightmare.
### The solution - AAM
AAM is a simple, elegant syntax that allows you to define bidirectional mappings in a single line. With AAM, you can write:
```aam
a = b
```
This single line creates a bidirectional mapping between `a` and `b`. You can look up `a` to get `b`, and look up `b` to get `a`. It's concise, clear, and eliminates the boilerplate.
AAM is designed to be concise, readable, and easy to use, stripping away the boilerplate so you can focus on the logic of your configuration.
## How idea was born
I was working on a project that required me to manage a large number of aliases. I was using TOML for my configuration files, and I found that it was very difficult to manage my aliases. I had to write a lot of boilerplate code to manage my aliases, and it was very easy to make mistakes. I wanted a better way to manage my aliases, and that is how I came up with the idea for AAM.
## Getting Started
Ready to simplify your configs? Check out the [Getting Started Guide](using/getting-started) to learn how to use AAM in your projects.