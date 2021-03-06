package(
    default_visibility = [
        "//visibility:public",
    ],
    licenses = ["notice"],  # Apache 2.0
)

cc_library(
    name = "op_builder",
    srcs = [
        "activation_builder.cc",
        "arg_min_max_builder.cc",
        "arithmetic_builder.cc",
        "concat_builder.cc",
        "conv_2d_builder.cc",
        "l2_normalization_builder.cc",
        "matmul_builder.cc",
        "neg_op_builder.cc",
        "op_builder.cc",
        "pad_builder.cc",
        "pool_2d_builder.cc",
        "reduce_builder.cc",
        "reshape_builder.cc",
        "resize_bilinear_builder.cc",
        "resize_nearest_neighbor_builder.cc",
        "softmax_builder.cc",
        "space_to_depth_builder.cc",
        "split_builder.cc",
        "transpose_builder.cc",
        "transpose_conv_2d_builder.cc",
    ],
    hdrs = [
        "activation_builder.h",
        "arg_min_max_builder.h",
        "arithmetic_builder.h",
        "concat_builder.h",
        "conv_2d_builder.h",
        "l2_normalization_builder.h",
        "matmul_builder.h",
        "neg_op_builder.h",
        "op_builder.h",
        "pad_builder.h",
        "pool_2d_builder.h",
        "reduce_builder.h",
        "reshape_builder.h",
        "resize_bilinear_builder.h",
        "resize_nearest_neighbor_builder.h",
        "softmax_builder.h",
        "space_to_depth_builder.h",
        "split_builder.h",
        "transpose_builder.h",
        "transpose_conv_2d_builder.h",
    ],
    tags = [
        "manual",
        "nobuilder",
    ],
    deps = [
        ":op_factory",
        "//tensorflow/lite:kernel_api",
        "//tensorflow/lite/c:common",
        "//tensorflow/lite/experimental/delegates/hexagon:hexagon_implementation",
        "//tensorflow/lite/experimental/delegates/hexagon/hexagon_nn:hexagon_nn_header",
        "//tensorflow/lite/kernels:kernel_util",
        "//tensorflow/lite/kernels:padding",
        "//tensorflow/lite/kernels/internal:optimized_base",
        "@hexagon_nn//:hexagon_nn_ops",
    ],
)

cc_library(
    name = "op_factory",
    hdrs = ["op_factory.h"],
    tags = [
        "manual",
        "nobuilder",
    ],
)
