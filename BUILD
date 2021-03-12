load("@io_bazel_rules_go//go:def.bzl", "go_binary", "go_library")
load("@bazel_gazelle//:def.bzl", "gazelle")

# gazelle:prefix github.com/fsouza/bazel-nolegacy_external_runfiles-repro
gazelle(name = "gazelle")

go_library(
    name = "bazel-nolegacy_external_runfiles-repro_lib",
    srcs = ["main.go"],
    importpath = "github.com/fsouza/bazel-nolegacy_external_runfiles-repro",
    visibility = ["//visibility:private"],
)

go_binary(
    name = "bazel-nolegacy_external_runfiles-repro",
    embed = [":bazel-nolegacy_external_runfiles-repro_lib"],
    visibility = ["//visibility:public"],
)
