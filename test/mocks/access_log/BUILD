licenses(["notice"])  # Apache 2

load(
    "//bazel:envoy_build_system.bzl",
    "envoy_cc_mock",
    "envoy_package",
)

envoy_package()

envoy_cc_mock(
    name = "access_log_mocks",
    srcs = ["mocks.cc"],
    hdrs = ["mocks.h"],
    deps = [
        "//include/envoy/access_log:access_log_interface",
        "//include/envoy/request_info:request_info_interface",
        "//test/mocks/filesystem:filesystem_mocks",
    ],
)
