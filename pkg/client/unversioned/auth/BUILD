package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_library(
    name = "go_default_library",
    srcs = ["clientauth.go"],
    tags = ["automanaged"],
    deps = ["//vendor:k8s.io/client-go/rest"],
)

go_test(
    name = "go_default_xtest",
    srcs = ["clientauth_test.go"],
    tags = ["automanaged"],
    deps = ["//pkg/client/unversioned/auth:go_default_library"],
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
)
