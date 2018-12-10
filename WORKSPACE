load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

# proto_library, cc_proto_library, and java_proto_library rules implicitly
# depend on @com_google_protobuf for protoc and proto runtimes.
# This statement defines the @com_google_protobuf repo.
http_archive(
    name = "com_google_protobuf",
    sha256 = "92f528f2f2b42b40c62fbced5fb34f4d6f4d80f79081e140794aad24df7fc1d0",
    strip_prefix = "protobuf-3.6.0.1",
    urls = ["https://github.com/google/protobuf/archive/v3.6.0.1.zip"],
)

http_archive(
    name = "com_github_gflags_gflags",
    sha256 = "94ad0467a0de3331de86216cbc05636051be274bf2160f6e86f07345213ba45b",
    strip_prefix = "gflags-77592648e3f3be87d6c7123eb81cbad75f9aef5a",
    url = "https://github.com/gflags/gflags/archive/77592648e3f3be87d6c7123eb81cbad75f9aef5a.zip",
)

http_archive(
    name = "com_github_google_glog",
    sha256 = "0dedfd600804986ee90e6f842a56d31cd680908596b097f8fad531eb6684d5da",
    strip_prefix = "glog-c72907c4a813fa724430f8692706cb639acdb756",
    url = "https://github.com/google/glog/archive/c72907c4a813fa724430f8692706cb639acdb756.zip",
)

new_http_archive(
    name = "com_github_tencent_rapidjson",
    build_file = "third_party/rapidjson.BUILD",
    sha256 = "8e00c38829d6785a2dfb951bb87c6974fa07dfe488aa5b25deec4b8bc0f6a3ab",
    strip_prefix = "rapidjson-1.1.0",
    url = "https://github.com/Tencent/rapidjson/archive/v1.1.0.zip",
)
