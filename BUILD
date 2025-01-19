exports_files(glob(["requirements*"]) + [
    "configure",
    "configure.py",
    "ACKNOWLEDGEMENTS",
    "LICENSE",
])

config_setting(
    name = "python_3_13",
    flag_values = {"python_version": "3.13"},
)

# Обновляем список поддерживаемых версий
SUPPORTED_PYTHON_VERSIONS = [
    "3.13",
    "3.12",
    "3.11",
    "3.10",
    "3.9",
]

# Добавляем зависимости для Python 3.13
py_library(
    name = "python_3_13_config",
    deps = [
        "@local_config_python//:python_headers",
        "@local_config_python//:numpy_headers",
    ],
    visibility = ["//visibility:public"],
)
