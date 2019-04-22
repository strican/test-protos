load("@io_bazel_rules_go//proto:def.bzl", "go_proto_library")

proto_library(
    name = "example_proto",
    srcs = ["example.proto"],
    visibility = ["//visibility:public"],
    deps = [
        "//api/common:bar_proto",
        "//api/common:foo_proto",
    ],
)

go_proto_library(
    name = "example_go_proto",
    compilers = ["@io_bazel_rules_go//proto:go_grpc"],
    importpath = "github.com/strican/test-protos/api/example",
    proto = ":example_proto",
    visibility = ["//visibility:public"],
    deps = [
        "//api/common:bar_go_proto",
        "//api/common:foo_go_proto",
    ],
)
