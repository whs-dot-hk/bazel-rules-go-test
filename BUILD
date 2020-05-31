load("@io_bazel_rules_go//go:def.bzl", "go_binary", "go_library")
load("@bazel_gazelle//:def.bzl", "gazelle")

# gazelle:prefix github.com/whs-dot-hk/bazel-rules-go-test
gazelle(name = "gazelle")

go_library(
    name = "go_default_library",
    srcs = ["main.go"],
    importpath = "github.com/whs-dot-hk/bazel-rules-go-test",
    visibility = ["//visibility:private"],
)

go_binary(
    name = "bazel-rules-go-test",
    embed = [":go_default_library"],
    visibility = ["//visibility:public"],
)
