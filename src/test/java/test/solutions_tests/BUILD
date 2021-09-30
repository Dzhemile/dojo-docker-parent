java_library(
    name = "solutions_tests",
    srcs = glob(["*.java"]),
    visibility = ["//src/test/java:__pkg__"],
    deps = ["//src/test/java/test/annotations:annotations",
            "//src/test/java/test/extensions:extensions",
            "//src/main/java/solutions:solutions",
            "@maven//:org_junit_jupiter_junit_jupiter_api",
            "@maven//:org_junit_jupiter_junit_jupiter_engine",
            "@maven//:org_junit_platform_junit_platform_launcher",
            "@maven//:org_junit_jupiter_junit_jupiter_params",
            "@maven//:org_junit_platform_junit_platform_runner",],
)