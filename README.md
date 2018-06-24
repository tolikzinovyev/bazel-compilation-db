# bazel-compilation-db
Generate `compile_commands.json` and run clang-tidy with [Bazel][bazel].
This is an adaptation of [Kythe][kythe]'s approach with a small patch to support the latest version of Bazel.

1. Append `WORKSPACE` to your repository's `WORKSPACE` file.
2. Copy `third_party` to your repository directory.
3. Optionally replace `'kind(cc_.*, //...)'` in `third_party/tools/generate_compilation_database.sh`.

To generate a `compile_commands.json` file in `$(bazel info execution_root)`, run `third_party/tools/generate_compilation_database.sh`.
To use `clang-tidy`, run `third_party/tools/clang_tidy.sh`.

Tested with Bazel 0.14.1.

[bazel]: https://bazel.build/
[kythe]: https://github.com/google/kythe
