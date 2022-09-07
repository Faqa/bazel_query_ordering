py_binary(
    name = "a",
    srcs = ["a.py"],
)

py_binary(
    name = "b",
    deps = [":a"],
    srcs = ["b.py"],
)

genquery(
    name = "b_query",
    expression = "deps(//:b)",
    scope = ["//:b"],
    opts = ["--notool_deps"],
)
