licenses(["notice"])  # Apache 2

load(
    "//bazel:envoy_build_system.bzl",
    "envoy_cc_library",
    "envoy_package",
)

envoy_package()

envoy_cc_library(
    name = "async_client_interface",
    hdrs = ["async_client.h"],
    deps = [
        ":status",
        "//include/envoy/common:optional",
        "//include/envoy/http:header_map_interface",
        "//include/envoy/tracing:http_tracer_interface",
        "//source/common/protobuf",
    ],
)

envoy_cc_library(
    name = "status",
    hdrs = ["status.h"],
)
