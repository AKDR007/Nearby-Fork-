cc_library(
    name = "sockets",
    srcs = [
        "client_socket.cc",
    ],
    hdrs = [
        "client_socket.h",
        "initial_data_provider.h",
    ],
    visibility = [
        "//connections:__subpackages__",
    ],
    deps = [
        "//internal/weave",
        "@com_google_absl//absl/random",
        "@com_google_absl//absl/status",
    ],
)

cc_test(
    name = "sockets_test",
    srcs = [
        "client_socket_test.cc",
    ],
    deps = [
        ":sockets",
        "//internal/platform:base",
        "//internal/platform:types",
        "//internal/platform/implementation/g3",  # build_cleaner: keep
        "@com_github_protobuf_matchers//protobuf-matchers",
        "@com_google_absl//absl/time",
        "@com_google_googletest//:gtest_main",
    ],
)