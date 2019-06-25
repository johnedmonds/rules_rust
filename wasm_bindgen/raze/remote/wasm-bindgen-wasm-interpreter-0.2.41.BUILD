"""
cargo-raze crate build file.

DO NOT EDIT! Replaced on runs of cargo-raze
"""
package(default_visibility = [
  # Public for visibility by "@raze__crate__version//" targets.
  #
  # Prefer access through "//wasm_bindgen/raze", which limits external
  # visibility to explicit Cargo.toml dependencies.
  "//visibility:public",
])

licenses([
  "notice", # "MIT,Apache-2.0"
])

load(
    "@io_bazel_rules_rust//rust:rust.bzl",
    "rust_library",
    "rust_binary",
    "rust_test",
)


# Unsupported target "smoke" with type "test" omitted

rust_library(
    name = "wasm_bindgen_wasm_interpreter",
    crate_root = "src/lib.rs",
    crate_type = "lib",
    edition = "2018",
    srcs = glob(["**/*.rs"]),
    deps = [
        "@raze__failure__0_1_5//:failure",
        "@raze__log__0_4_6//:log",
        "@raze__walrus__0_5_0//:walrus",
    ],
    rustc_flags = [
        "--cap-lints=allow",
    ],
    version = "0.2.41",
    crate_features = [
    ],
)

