"""
@generated
cargo-raze crate build file.

DO NOT EDIT! Replaced on runs of cargo-raze
"""

# buildifier: disable=load
load(
    "@io_bazel_rules_rust//rust:rust.bzl",
    "rust_binary",
    "rust_library",
    "rust_test",
)

# buildifier: disable=load
load("@bazel_skylib//lib:selects.bzl", "selects")

package(default_visibility = [
    # Public for visibility by "@raze__crate__version//" targets.
    #
    # Prefer access through "//proto/raze", which limits external
    # visibility to explicit Cargo.toml dependencies.
    "//visibility:public",
])

licenses([
    "notice",  # MIT from expression "MIT OR Apache-2.0"
])

# Generated targets

# buildifier: leave-alone
rust_library(
    name = "crossbeam_deque",
    crate_type = "lib",
    deps = [
        "@rules_rust_proto__crossbeam_epoch__0_8_2//:crossbeam_epoch",
        "@rules_rust_proto__crossbeam_utils__0_7_2//:crossbeam_utils",
        "@rules_rust_proto__maybe_uninit__2_0_0//:maybe_uninit",
    ],
    srcs = glob(["**/*.rs"]),
    crate_root = "src/lib.rs",
    edition = "2015",
    rustc_flags = [
        "--cap-lints=allow",
    ],
    version = "0.7.3",
    tags = [
        "cargo-raze",
        "manual",
    ],
    crate_features = [
    ],
)
# Unsupported target "fifo" with type "test" omitted
# Unsupported target "injector" with type "test" omitted
# Unsupported target "lifo" with type "test" omitted
# Unsupported target "steal" with type "test" omitted
