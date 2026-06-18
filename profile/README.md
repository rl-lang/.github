<div align="center">
  <img src="https://raw.githubusercontent.com/rl-lang/rl-lang/main/logo-circle.svg" width="200">
  <h1>rl-lang</h1>
  <p>A language that is fast to write, simple to read, built in Rust from the ground up.</p>
</div>

---

## Repositories

| Repo | Description |
|------|-------------|
| [rl-lang](https://github.com/rl-lang/rl-lang) | The main interpreter, stdlib, TUI REPL, and CLI |
| [tree-sitter-rl](https://github.com/rl-lang/tree-sitter-rl) | Tree-sitter grammar for Neovim, Helix, Zed, and more |
| [rl-vscode](https://github.com/rl-lang/rl-vscode) | VS Code extension for syntax highlighting |
| [dsl-html](https://github.com/rl-lang/dsl-html) | DSL-based static site generator written in rl-lang |
| [rl-check](https://github.com/rl-lang/rl-check) | GitHub Action for rl-lang CI integration |

## Quick look

```rl
get println, len from std::io
get pow, mod, factorial, fibonacci, is_prime from std::math
get PI from std::math::consts

fn collatz(int n) {
    dec int steps = 0
    while (n != 1) {
        if (mod(n, 2) == 0) {
            n = n / 2
        } else {
            n = n * 3 + 1
        }
        steps += 1
    }
    return steps
}

println(factorial(10))    // 3628800
println(fibonacci(15))    // 610
println(is_prime(97))     // true
println(collatz(27))      // 111
```

## Installation

```bash
cargo install rl-lang
```

## Links

- [Documentation & Wiki](https://github.com/rl-lang/rl-lang/wiki)
- [Changelog](https://github.com/rl-lang/rl-lang/releases)
- [Contributing](https://github.com/rl-lang/rl-lang/blob/main/CONTRIBUTING.md)

## License

MIT or Apache 2.0 at your option.
