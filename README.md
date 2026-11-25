# Saule examples

Example projects for [Saule](https://github.com/lauriszz123/saule), a
statically typed, class-oriented scripting language. Each folder is an
ordinary Saule project you can read and run.

```sh
git clone https://github.com/lauriszz123/saule-examples.git
cd saule-examples/bf
saule run -- -d
```

`saule` itself is installed from the
[Saule repository](https://github.com/lauriszz123/saule#readme); the
[documentation](https://lauriszz123.github.io/saule/examples/) walks through
most of these file by file.

## The projects

Grouped by what you need to know to read them, not by how long they are.

### Simple

| Project | What it shows |
| --- | --- |
| [`fs-info-example`](fs-info-example) | Inspects a path with `Os.fsInfo`: nullable returns, and `match` over an enum. |
| [`todo-app`](todo-app) | A command-line app: arguments, JSON persistence through a library dependency, `match` over subcommands. |
| [`json_usage`](json_usage) | Reading and writing JSON with the `json` library below. |

### Intermediate

| Project | What it shows |
| --- | --- |
| [`vector-math`](vector-math) | Operator overloading: a `Vec2` that adds, compares and prints like a number. |
| [`bitwise-flags`](bitwise-flags) | The bitwise operators: a permission flag set, and a colour packed into one integer. |
| [`bf`](bf) | A Brainfuck interpreter in about 240 lines. |
| [`json`](json) | A JSON library, written in Saule: what `todo-app` and `json_usage` depend on. |
| [`markdown`](markdown) | A Markdown parser as a library, used by `md-viewer`. |

### Advanced

| Project | What it shows |
| --- | --- |
| [`wrapper-types`](wrapper-types) | Target-typed construction (`Assignable<T>`) and index overloading (`OpIndex`, `OpNewIndex`). |
| [`ui-blocks`](ui-blocks) | A small declarative UI toolkit drawn to the terminal, with children given as trailing blocks. |
| [`coroutines`](coroutines) | Lazy streams, a tokenizer and parser, and a cooperative scheduler, all on coroutines. |

### With a window

These draw with [Shine](https://github.com/lauriszz123/saule-shine), Saule's
graphics package, which `saule install` fetches and builds
([Rust](https://rustup.rs) is needed for that).

| Project | What it shows |
| --- | --- |
| [`toying`](toying) | A window, and a rectangle that follows the mouse. |
| [`native-package`](native-package) | Calling a native package from Saule: keyboard, images, a game loop. |
| [`roguelike`](roguelike) | A top-down roguelite, drawn and heard with Shine. |
| [`UI Project`](UI%20Project) | An app built on [saule-uikit](https://github.com/lauriszz123/saule-uikit). |
| [`md-viewer`](md-viewer) | A Markdown viewer on uikit and the `markdown` library. |

## Running them all

The Saule repository carries this one as its `examples/` folder and runs
every project as part of its tests (`run_examples.sh` there).

## License

MIT, as Saule is: see [LICENSE](LICENSE).
