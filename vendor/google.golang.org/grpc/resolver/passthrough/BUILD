load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["passthrough.go"],
    importmap = "k8s.io/kubernetes/vendor/google.golang.org/grpc/resolver/passthrough",
    importpath = "google.golang.org/grpc/resolver/passthrough",
    visibility = ["//visibility:public"],
    deps = ["//vendor/google.golang.org/grpc/internal/resolver/passthrough:go_default_library"],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
