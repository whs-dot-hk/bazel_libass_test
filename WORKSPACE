load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

# local_repository(
#     name = "rules_foreign_cc",
#     path = "../rules_foreign_cc",
# )

http_archive(
    name = "rules_foreign_cc",
    strip_prefix = "rules_foreign_cc-master",
    url = "https://github.com/bazelbuild/rules_foreign_cc/archive/master.zip",
)

load("@rules_foreign_cc//:workspace_definitions.bzl", "rules_foreign_cc_dependencies")

rules_foreign_cc_dependencies()

http_archive(
    name = "freetype2",
    build_file = "@//:BUILD.freetype2",
    strip_prefix = "freetype-2.10.2",
    urls = ["https://download.savannah.gnu.org/releases/freetype/freetype-2.10.2.tar.gz"],
)

http_archive(
    name = "fribidi",
    build_file = "@//:BUILD.fribidi",
    strip_prefix = "fribidi-1.0.10",
    urls = ["https://github.com/fribidi/fribidi/releases/download/v1.0.10/fribidi-1.0.10.tar.xz"],
)

http_archive(
    name = "fontconfig",
    build_file = "@//:BUILD.fontconfig",
    strip_prefix = "fontconfig-2.13.1",
    urls = ["https://www.freedesktop.org/software/fontconfig/release/fontconfig-2.13.1.tar.gz"],
)

http_archive(
    name = "util_linux",
    build_file = "@//:BUILD.util_linux",
    strip_prefix = "util-linux-2.36",
    urls = ["https://www.kernel.org/pub/linux/utils/util-linux/v2.36/util-linux-2.36.tar.gz"],
)

http_archive(
    name = "expat",
    build_file = "@//:BUILD.expat",
    strip_prefix = "expat-2.2.9",
    urls = ["https://github.com/libexpat/libexpat/releases/download/R_2_2_9/expat-2.2.9.tar.gz"],
)

http_archive(
    name = "libass",
    build_file = "@//:BUILD.libass",
    strip_prefix = "libass-0.14.0",
    urls = ["https://github.com/libass/libass/releases/download/0.14.0/libass-0.14.0.tar.gz"],
)
