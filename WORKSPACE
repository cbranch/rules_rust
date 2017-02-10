workspace(name = "io_bazel_rules_rust")

local_repository(
    name = "examples",
    path = "examples",
)

# TODO: Move this to examples/WORKSPACE when recursive repositories are enabled.
load("//rust:rust.bzl", "rust_repositories")

rust_repositories()

# Used for documenting Rust rules.
git_repository(
    name = "io_bazel_rules_sass",
    remote = "https://github.com/bazelbuild/rules_sass.git",
    tag = "0.0.2",
)

load("@io_bazel_rules_sass//sass:sass.bzl", "sass_repositories")

sass_repositories()

git_repository(
    name = "io_bazel_skydoc",
    remote = "https://github.com/bazelbuild/skydoc.git",
    tag = "0.1.2",
)

load("@io_bazel_skydoc//skylark:skylark.bzl", "skydoc_repositories")

skydoc_repositories()