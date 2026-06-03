# test

Lightweight test runner with assertion helpers. Workflow: build a List of `TestCase`s, hand it to `test.run_all(...)`. Each test is a `(name, lambda)` pair. The runner executes every case, prints a pa

This package is also bundled with the Quirk compiler at
`<QUIRK_HOME>/packages/test/`, so `use test` works out of the box on a
fresh install. This repo is the canonical home — when you want a version
newer than the one your compiler shipped with, install it explicitly:

```bash
quirk pkg install test             # latest tag from this repo
quirk pkg install test@1.0.0       # pinned
```

The compiler-shipped registry maps the bare name `test` to this repo
(since v1.4.0), so no `quirk pkg registry add` is needed.

## Origin

Split from `quirk-compiler/packages/test/` in compiler v1.5.0 as part of
the stdlib-in-independent-repos rollout. Source history before that lives
in [AlexVachon/quirk](https://github.com/AlexVachon/quirk).

## License

MIT (see [`LICENSE`](LICENSE)).
