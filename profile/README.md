<div align="center">
  <img src="https://raw.githubusercontent.com/rl-lang/rl-lang/main/assets/logo-circle.svg" width="200">
  <h1>rl-lang</h1>
  <p>Fast to write. Simple to read. Built in Rust from the ground up.</p>
</div>

---

## Quick look

```rl
get println from std::io
get len from std
get pow, mod, factorial, fibonacci, is_prime from std::math
get PI from std::math::consts

fn collatz(int n)
{
    dec int steps = 0
    while (n != 1)
    {
        if (mod(n, 2)? == 0)
        {
            n = n / 2
        }
        else
        {
            n = n * 3 + 1
        }
        steps += 1
    }
    return steps
}

println(factorial(10)?)    // 3628800
println(fibonacci(15)?)    // 610
println(is_prime(97)?)     // true
println(collatz(27))       // 111
```

## Repositories

### Core

| Repo | Description |
|------|-------------|
| [rl-lang](https://github.com/rl-lang/rl-lang) | The language itself: interpreter, stdlib, CLI, C transpiler, REPL, LSP, and docs |
| [the-book](https://github.com/rl-lang/the-book) | The official language reference and documentation |
| [e-rl](https://github.com/rl-lang/e-rl) | rl-lang for embedded systems |

### CI actions

| Repo | Description |
|------|-------------|
| [rl-setup](https://github.com/rl-lang/rl-setup) | Install the RL toolchain in CI. Base action the rest build on |
| [rl-check](https://github.com/rl-lang/rl-check) | Type-check RL sources in CI |
| [rl-test](https://github.com/rl-lang/rl-test) | Run the RL test runner in CI |
| [rl-transpile](https://github.com/rl-lang/rl-transpile) | Transpile RL to C in CI |
| [rl-format](https://github.com/rl-lang/rl-format) | Enforce `rl format` style in CI |
| [rl-package](https://github.com/rl-lang/rl-package) | Build distributable RL binaries in CI |

### Editors

| Repo | Description |
|------|-------------|
| [vscode-rl-lang](https://github.com/rl-lang/vscode-rl-lang) | Full VS Code support: highlighting, LSP, run/check/format/package commands |
| [rl-zed-extension](https://github.com/rl-lang/rl-zed-extension) | RL support for Zed: tree-sitter highlighting plus `rlsp` diagnostics |
| [rl-textmate](https://github.com/rl-lang/rl-textmate) | Canonical TextMate grammar (`.rl`) shared by VS Code, JetBrains, and Linguist |
| [tree-sitter-rl](https://github.com/rl-lang/tree-sitter-rl) | Tree-sitter grammar for Helix, Neovim, Zed, and more |

### Systems

| Repo | Description |
|------|-------------|
| [rlos](https://github.com/rl-lang/rlos) | Bootable Linux userspace experiment running RL programs as PID-1-and-up |
| [core-utils](https://github.com/rl-lang/core-utils) | Unix core utilities reimplemented in RL |

### Programs and libraries

| Repo | Description |
|------|-------------|
| [rl-examples](https://github.com/rl-lang/rl-examples) | Small RL programs too focused for their own repo |
| [rlchase](https://github.com/rl-lang/rlchase) | Terminal maze-chase game built in RL |
| [dsl-html](https://github.com/rl-lang/dsl-html) | HTML and CSS static site generator written in RL |
| [rl-website](https://github.com/rl-lang/rl-website) | The rl-lang landing page, written in RL |

### Meta

| Repo | Description |
|------|-------------|
| [.github](https://github.com/rl-lang/.github) | Org profile, templates, and shared workflows (this repo) |

### Packaging

| Repo | Description |
|------|-------------|
| [rl-pack-linux](https://github.com/rl-lang/rl-pack-linux) | Linux packaging: deb, rpm, AUR, Gentoo, Nix, Snap, Flatpak |
| [homebrew-rl](https://github.com/rl-lang/homebrew-rl) | Homebrew tap: `brew tap rl-lang/rl && brew install rl-lang` |
| [rl-pack-windows](https://github.com/rl-lang/rl-pack-windows) | Windows packaging: Chocolatey and WinGet |

## Installation

Prebuilt binaries ship with every [release](https://github.com/rl-lang/rl-lang/releases):

```bash
curl -fsSL https://raw.githubusercontent.com/rl-lang/rl-lang/main/install.sh -o install.sh
bash install.sh
```

## Links

- [Documentation](https://rl-lang.github.io/the-book/)
- [API docs](https://rl-lang.github.io/rl-lang/)
- [Changelog](https://github.com/rl-lang/rl-lang/releases)
- [Contributing](https://github.com/rl-lang/rl-lang/blob/main/CONTRIBUTING.md)
- [Discord](https://discord.gg/AHvVbKjJN7)

## License

MIT or Apache 2.0 at your option.
