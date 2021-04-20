licenses(["notice"])  # Apache 2

cc_library(
    name = "host-ssl-1-1",
    srcs = [
        "lib/libcrypto.so.1.1",
        "lib/libssl.so.1.1",
    ],
    hdrs = glob(["include/openssl/*.h"]),
    includes = ["include"],
    linkstatic = False,
    visibility = ["//visibility:public"],
)

alias(
    name = "ssl",
    actual = "host-ssl-1-1",
    visibility = ["//visibility:public"],
)
