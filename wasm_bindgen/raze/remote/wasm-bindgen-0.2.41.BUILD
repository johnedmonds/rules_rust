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


# Unsupported target "build-script-build" with type "custom-build" omitted
# Unsupported target "headless" with type "test" omitted
# Unsupported target "non_wasm" with type "test" omitted
# Unsupported target "std-crate-no-std-dep" with type "test" omitted
# Unsupported target "unwrap_throw" with type "test" omitted
# Unsupported target "wasm" with type "test" omitted

rust_library(
    name = "wasm_bindgen",
    crate_root = "src/lib.rs",
    crate_type = "lib",
    edition = "2018",
    srcs = glob(["**/*.rs"]),
    deps = [
        "@raze__wasm_bindgen_macro__0_2_41//:wasm_bindgen_macro",
    ],
    rustc_flags = [
        "--cap-lints=allow",
    ],
    version = "0.2.41",
    crate_features = [
        "default",
        "spans",
        "std",
        "wasm-bindgen-macro",
    ],
)

