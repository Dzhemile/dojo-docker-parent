java_binary(
    name = "tests",
    srcs = glob(["*.java"]),
    main_class = "TestMain",
    deps = [
            "//src/main/java/model:model",
            "//src/main/java/service:service",
            "//src/test/java/test/extensions:extensions",
            "//src/test/java/test/solutions_tests:solutions_tests",
            "@maven//:org_junit_platform_junit_platform_launcher",
            "@maven//:com_squareup_okhttp3_okhttp",
            '@maven//:org_junit_platform_junit_platform_engine'
]
)
