#package(default_visibility = ["//visibility:public"])
load(
    "@io_bazel_rules_docker//container:container.bzl",
    "container_bundle",
    "container_flatten",
    "container_image",
    "container_import",
)

container_image(
    name = "hello",
    base = "@ubuntu//image:image.tar",
    files = ["entrypoint.sh", "hello.sh"],
    mode = "0744",
    #cmd = ["adduser", "ali"],
    entrypoint = "/entrypoint.sh",
    
)
