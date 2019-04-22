load("@io_bazel_rules_go//proto:def.bzl", "go_proto_library")

proto_library(
    name = "bar_proto",
    srcs = ["bar.proto"],
    visibility = ["//visibility:public"],
)

proto_library(
    name = "baz_proto",
    srcs = ["baz.proto"],
    visibility = ["//visibility:public"],
)

proto_library(
    name = "foo_proto",
    srcs = ["foo.proto"],
    visibility = ["//visibility:public"],
)

go_proto_library(
    name = "bar_go_proto",
    importpath = "github.com/strican/test-protos/api/common",
    proto = ":bar_proto",
    visibility = ["//visibility:public"],
)

go_proto_library(
    name = "baz_go_proto",
    importpath = "github.com/strican/test-protos/api/common",
    proto = ":baz_proto",
    visibility = ["//visibility:public"],
)

go_proto_library(
    name = "foo_go_proto",
    importpath = "github.com/strican/test-protos/api/common",
    proto = ":foo_proto",
    visibility = ["//visibility:public"],
)
