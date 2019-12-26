load("@io_bazel_rules_closure//closure:defs.bzl", "closure_js_library")

package(
    default_visibility = [
    ],
)

licenses(["notice"])  # Apache 2.0

closure_js_library(
    name = "defines",
    srcs = ["defines.js"],
    deps = [
    ],
)

closure_js_library(
    name = "internal_checks",
    srcs = ["internal_checks.js"],
    deps = [
        ":defines",
    ],
)

closure_js_library(
    name = "equivalence",
    srcs = ["equivalence.js"],
    deps = [
    ],
)

closure_js_library(
    name = "hashing",
    srcs = ["hashing.js"],
    deps = [
        ":internal_checks",
    ],
)

closure_js_library(
    name = "jspbkernel",
    srcs = ["jspbkernel.js"],
    deps = [
        ":bytestring",
        ":equivalence",
        ":fieldaccessor",
        ":hashing",
        ":internal_checks",
        ":listview",
    ],
)

closure_js_library(
    name = "listview",
    srcs = ["listview.js"],
    deps = [
        ":internal_checks",
    ],
)

closure_js_library(
    name = "bytestring",
    srcs = ["bytestring.js"],
    deps = [
        ":hashing",
        ":internal_checks",
    ],
)

closure_js_library(
    name = "fieldaccessor",
    srcs = ["fieldaccessor.js"],
    deps = [
        ":bytestring",
        ":internal_checks",
        ":listview",
    ],
)

closure_js_library(
    name = "message",
    srcs = ["message.js"],
    deps = [
        ":listview",
    ],
)

closure_js_library(
    name = "internal_message",
    srcs = ["internal_message.js"],
    deps = [
        ":bytestring",
        ":internal_checks",
        ":jspbkernel",
        ":listview",
        ":message",
    ],
)