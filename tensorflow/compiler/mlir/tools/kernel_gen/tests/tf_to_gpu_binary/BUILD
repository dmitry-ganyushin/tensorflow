load("//tensorflow/compiler/mlir:glob_lit_test.bzl", "glob_lit_tests")

package(licenses = ["notice"])

glob_lit_tests(
    data = [
        "//tensorflow/compiler/mlir/tools/kernel_gen:tf_to_gpu_binary",
        "@llvm-project//mlir:run_lit.sh",
    ],
    default_tags = [
        # We need access to the CUDA SDK.
        "gpu",
        "no_rocm",
    ],
    driver = "//tensorflow/compiler/mlir:run_lit.sh",
    test_file_exts = ["mlir"],
)
