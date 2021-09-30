load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

RULES_JVM_EXTERNAL_TAG = "4.0"
RULES_JVM_EXTERNAL_SHA = "31701ad93dbfe544d597dbe62c9a1fdd76d81d8a9150c2bf1ecf928ecdf97169"

http_archive(
    name = "rules_jvm_external",
    strip_prefix = "rules_jvm_external-%s" % RULES_JVM_EXTERNAL_TAG,
    sha256 = RULES_JVM_EXTERNAL_SHA,
    url = "https://github.com/bazelbuild/rules_jvm_external/archive/%s.zip" % RULES_JVM_EXTERNAL_TAG,
)

load("@rules_jvm_external//:defs.bzl", "maven_install")

maven_install(
    name = "maven",
    artifacts = [
        "org.junit.jupiter:junit-jupiter-api:5.7.1",
        "org.junit.jupiter:junit-jupiter-engine:5.7.1",
        "org.junit.platform:junit-platform-launcher:1.7.1",
        "org.junit.jupiter:junit-jupiter-params:5.7.1",
        "org.junit.platform:junit-platform-runner:1.7.1",
        "com.squareup.okhttp3:okhttp:4.9.1",
        "com.googlecode.json-simple:json-simple:1.1.1",
        # https://mvnrepository.com/artifact/org.junit.platform/junit-platform-engine
        'org.junit.platform:junit-platform-engine:jar:1.7.1'

    ],
    repositories = [
        "https://repo1.maven.org/maven2"
    ],
    fetch_sources = True,   # Fetch source jars. Defaults to False.
)