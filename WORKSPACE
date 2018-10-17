load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "io_bazel_rules_go",
    urls = ["https://github.com/bazelbuild/rules_go/releases/download/0.15.4/rules_go-0.15.4.tar.gz"],
    sha256 = "7519e9e1c716ae3c05bd2d984a42c3b02e690c5df728dc0a84b23f90c355c5a1",
)

http_archive(
    name = "bazel_gazelle",
    urls = ["https://github.com/bazelbuild/bazel-gazelle/releases/download/0.15.0/bazel-gazelle-0.15.0.tar.gz"],
    sha256 = "6e875ab4b6bf64a38c352887760f21203ab054676d9c1b274963907e0768740d",
)

load("@io_bazel_rules_go//go:def.bzl", "go_rules_dependencies", "go_register_toolchains")

go_rules_dependencies()

go_register_toolchains()

load("@bazel_gazelle//:deps.bzl", "gazelle_dependencies", "go_repository")

gazelle_dependencies()

go_repository(
    name = "com_github_burntsushi_toml",
    importpath = "github.com/BurntSushi/toml",
    tag = "v0.3.0",
)

go_repository(
    name = "com_github_fatih_color",
    importpath = "github.com/fatih/color",
    tag = "v1.7.0",
)

go_repository(
    name = "com_github_fatih_structtag",
    importpath = "github.com/fatih/structtag",
    tag = "v1.0.0",
)

go_repository(
    name = "com_github_mattn_go_colorable",
    importpath = "github.com/mattn/go-colorable",
    tag = "v0.0.9",
)

go_repository(
    name = "com_github_mattn_go_isatty",
    importpath = "github.com/mattn/go-isatty",
    tag = "v0.0.4",
)

go_repository(
    name = "com_github_mattn_go_runewidth",
    importpath = "github.com/mattn/go-runewidth",
    tag = "v0.0.3",
)

go_repository(
    name = "com_github_mgechev_dots",
    commit = "8e09d8ea2757",
    importpath = "github.com/mgechev/dots",
)

go_repository(
    name = "com_github_olekukonko_tablewriter",
    commit = "be2c049b30cc",
    importpath = "github.com/olekukonko/tablewriter",
)

go_repository(
    name = "com_github_pkg_errors",
    importpath = "github.com/pkg/errors",
    tag = "v0.8.0",
)

go_repository(
    name = "org_golang_x_sys",
    commit = "d0be0721c37e",
    importpath = "golang.org/x/sys",
)

go_repository(
    name = "org_golang_x_tools",
    commit = "677d2ff680c1",
    importpath = "golang.org/x/tools",
)
