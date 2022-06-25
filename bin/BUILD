package(default_visibility = ["//visibility:public"])
load("@requirements//:requirements.bzl", "requirement")

py_binary (
    name = "main",
    srcs = glob(["main.py"]),
)

py_test(
    name = "test_main",
    srcs = ["test_main.py"],
    deps = [
      "main",
      requirement("testify"),
    ],
)

test_suite(
    name = "all_tests",
    tests = [
        "test_main",
    ],
)
