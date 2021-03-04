load("@build_bazel_rules_android//android:rules.bzl", "android_binary")
load("@io_bazel_rules_kotlin//kotlin:kotlin.bzl", "kt_android_library")

android_binary(
    name = "app",
    srcs = glob(["src/main/java/**/*.java"]),
    custom_package = "ir.beigirad.bazelexample",
    manifest = "src/main/AndroidManifest.xml",
    manifest_values = {
        "minSdkVersion": "16",
    },
    resource_files = glob(["src/main/res/**"]),
    deps = [
        "@maven//:androidx_appcompat_appcompat",
        "@maven//:androidx_constraintlayout_constraintlayout",
        "@maven//:com_google_android_material_material",
    ],
)

kt_android_library(
    name = "app_kt",
    srcs = glob(["src/main/java/**/*.kt"]),
    custom_package = "ir.beigirad.bazelexample",
    manifest = "src/main/AndroidManifest.xml",
    resource_files = glob(["src/main/res/**"]),
    deps = [
    ],
)
