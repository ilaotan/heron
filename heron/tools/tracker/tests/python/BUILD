package(default_visibility = ["//visibility:public"])

pex_library(
    name = "mock_proto",
    srcs = ["mock_proto.py"],
    deps = [
        "//heron/proto:proto-py",
        "//heronpy/api:heron-python-py",
    ],
)

pex_pytest(
    name = "topology_unittest",
    size = "small",
    srcs = [
        "mock_proto.py",
        "topology_unittest.py",
    ],
    reqs = [
        "pytest==3.2.2",
    ],
    deps = [
        "//heron/proto:proto-py",
        "//heron/tools/tracker/src/python:tracker-py",
        "//heronpy/api:heron-python-py",
    ],
)

pex_pytest(
    name = "query_operator_unittest",
    size = "small",
    srcs = ["query_operator_unittest.py"],
    reqs = [
        "pytest==3.2.2",
    ],
    deps = [
        "//heron/tools/tracker/src/python:tracker-py",
    ],
)

pex_pytest(
    name = "query_unittest",
    size = "small",
    srcs = ["query_unittest.py"],
    reqs = [
        "pytest==3.2.2",
    ],
    deps = [
        "//heron/tools/tracker/src/python:tracker-py",
    ],
)

pex_pytest(
    name = "tracker_unittest",
    size = "small",
    srcs = [
        "mock_proto.py",
        "tracker_unittest.py",
    ],
    reqs = [
        "pytest==3.2.2",
    ],
    deps = [
        "//heron/proto:proto-py",
        "//heron/tools/tracker/src/python:tracker-py",
    ],
)
