# Tests of TensorFlow array ops kernels written using the Python API.

load("//tensorflow:tensorflow.bzl", "cuda_py_test")

package(
    default_visibility = ["//tensorflow:internal"],
    licenses = ["notice"],  # Apache 2.0
)

cuda_py_test(
    name = "batch_gather_op_test",
    srcs = ["batch_gather_op_test.py"],
    xla_enable_strict_auto_jit = False,  # b/162351094
    deps = [
        "//tensorflow/python:array_ops",
        "//tensorflow/python:client_testlib",
        "//tensorflow/python:constant_op",
        "//tensorflow/python:dtypes",
        "@absl_py//absl/testing:parameterized",
    ],
)
