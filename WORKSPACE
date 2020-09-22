load(
    "@bazel_tools//tools/build_defs/repo:http.bzl",
    "http_archive",
    "http_file",
)
load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")

# Additional bazel rules

http_archive(
    name = "io_bazel_rules_go",
    sha256 = "38392eb0617c1a9fdff17c4a284f012da13e4feefbaf87d04b3579b107902e9b",
    urls = [
        "https://mirror.bazel.build/github.com/bazelbuild/rules_go/releases/download/v0.22.8/rules_go-v0.22.8.tar.gz",
        "https://github.com/bazelbuild/rules_go/releases/download/v0.22.8/rules_go-v0.22.8.tar.gz",
    ],
)

http_archive(
    name = "bazel_gazelle",
    sha256 = "41bff2a0b32b02f20c227d234aa25ef3783998e5453f7eade929704dcff7cd4b",
    urls = [
        "https://storage.googleapis.com/bazel-mirror/github.com/bazelbuild/bazel-gazelle/releases/download/v0.19.0/bazel-gazelle-v0.19.0.tar.gz",
        "https://github.com/bazelbuild/bazel-gazelle/releases/download/v0.19.0/bazel-gazelle-v0.19.0.tar.gz",
    ],
)

http_archive(
    name = "com_google_protobuf",
    sha256 = "cd218dc003eacc167e51e3ce856f6c2e607857225ef86b938d95650fcbb2f8e4",
    strip_prefix = "protobuf-6d4e7fd7966c989e38024a8ea693db83758944f1",
    # version 3.10.0
    urls = [
        "https://github.com/google/protobuf/archive/6d4e7fd7966c989e38024a8ea693db83758944f1.zip",
        "https://storage.googleapis.com/builddeps/cd218dc003eacc167e51e3ce856f6c2e607857225ef86b938d95650fcbb2f8e4",
    ],
)

http_archive(
    name = "com_github_bazelbuild_buildtools",
    sha256 = "875d0c49953e221cfc35d2a3846e502f366dfa4024b271fa266b186ca4664b37",
    strip_prefix = "buildtools-5bcc31df55ec1de770cb52887f2e989e7068301f",
    # version 0.29.0
    url = "https://github.com/bazelbuild/buildtools/archive/5bcc31df55ec1de770cb52887f2e989e7068301f.zip",
)

http_archive(
    name = "io_bazel_rules_docker",
    sha256 = "3efbd23e195727a67f87b2a04fb4388cc7a11a0c0c2cf33eec225fb8ffbb27ea",
    strip_prefix = "rules_docker-0.14.2",
    urls = [
        "https://github.com/bazelbuild/rules_docker/releases/download/v0.14.2/rules_docker-v0.14.2.tar.gz",
        "https://storage.googleapis.com/builddeps/3efbd23e195727a67f87b2a04fb4388cc7a11a0c0c2cf33eec225fb8ffbb27ea",
    ],
)

http_archive(
    name = "com_github_atlassian_bazel_tools",
    sha256 = "e4737fd3636d23f12cd3f9880b1cfa75c1bbdd4a967852785e227f3b0ab11844",
    strip_prefix = "bazel-tools-7d296003f478325b4a933c2b1372426d3a0926f0",
    urls = [
        "https://github.com/atlassian/bazel-tools/archive/7d296003f478325b4a933c2b1372426d3a0926f0.zip",
        "https://storage.googleapis.com/builddeps/e4737fd3636d23f12cd3f9880b1cfa75c1bbdd4a967852785e227f3b0ab11844",
    ],
)

# Libvirt dependencies
http_file(
    name = "libvirt_libs",
    sha256 = "59f119cf1347d07c0fa048d0c85b3e0e4a34987c481b26229d0c86fc4a8b0a22",
    urls = [
        "https://copr-be.cloud.fedoraproject.org/results/%40virtmaint-sig/for-kubevirt/fedora-31-x86_64/01113510-libvirt/libvirt-libs-5.0.0-2.fc31.x86_64.rpm",
        "https://storage.googleapis.com/builddeps/59f119cf1347d07c0fa048d0c85b3e0e4a34987c481b26229d0c86fc4a8b0a22",
    ],
)

http_file(
    name = "libvirt_devel",
    sha256 = "bf566d24c6657c8c28cf266c8ba796436b605dfa8c5162e1add4c8a56f0706b0",
    urls = [
        "https://copr-be.cloud.fedoraproject.org/results/%40virtmaint-sig/for-kubevirt/fedora-31-x86_64/01113510-libvirt/libvirt-devel-5.0.0-2.fc31.x86_64.rpm",
        "https://storage.googleapis.com/builddeps/bf566d24c6657c8c28cf266c8ba796436b605dfa8c5162e1add4c8a56f0706b0",
    ],
)

# Disk images
http_file(
    name = "alpine_image",
    sha256 = "5a4b2588afd32e7024dd61d9558b77b03a4f3189cb4c9fc05e9e944fb780acdd",
    urls = [
        "http://dl-cdn.alpinelinux.org/alpine/v3.7/releases/x86_64/alpine-virt-3.7.0-x86_64.iso",
        "https://storage.googleapis.com/builddeps/5a4b2588afd32e7024dd61d9558b77b03a4f3189cb4c9fc05e9e944fb780acdd",
    ],
)

http_file(
    name = "alpine_image_ppc64le",
    sha256 = "4b1d35e7cc9f5e1f5774ed9ea47c85893f20dc8713625e1f8fa7fbddca243a15",
    urls = [
        "http://dl-cdn.alpinelinux.org/alpine/v3.7/releases/ppc64le/alpine-vanilla-3.7.0-ppc64le.iso",
        "https://storage.googleapis.com/builddeps/4b1d35e7cc9f5e1f5774ed9ea47c85893f20dc8713625e1f8fa7fbddca243a15",
    ],
)

http_file(
    name = "cirros_image",
    sha256 = "a8dd75ecffd4cdd96072d60c2237b448e0c8b2bc94d57f10fdbc8c481d9005b8",
    urls = [
        "https://download.cirros-cloud.net/0.4.0/cirros-0.4.0-x86_64-disk.img",
        "https://storage.googleapis.com/builddeps/a8dd75ecffd4cdd96072d60c2237b448e0c8b2bc94d57f10fdbc8c481d9005b8",
    ],
)

http_file(
    name = "cirros_image_ppc64le",
    sha256 = "175063e409f4019acb760478eb1a94819628a1bec9376d26d3aa333449fe061d",
    urls = [
        "https://download.cirros-cloud.net/0.4.0/cirros-0.4.0-ppc64le-disk.img",
        "https://storage.googleapis.com/builddeps/175063e409f4019acb760478eb1a94819628a1bec9376d26d3aa333449fe061d",
    ],
)

http_file(
    name = "fedora_image",
    sha256 = "423a4ce32fa32c50c11e3d3ff392db97a762533b81bef9d00599de518a7469c8",
    urls = [
        "https://download.fedoraproject.org/pub/fedora/linux/releases/32/Cloud/x86_64/images/Fedora-Cloud-Base-32-1.6.x86_64.qcow2",
        "https://storage.googleapis.com/builddeps/423a4ce32fa32c50c11e3d3ff392db97a762533b81bef9d00599de518a7469c8",
    ],
)

http_file(
    name = "fedora_image_ppc64le",
    sha256 = "dd989a078d641713c55720ba3e4320b204ade6954e2bfe4570c8058dc36e2e5d",
    urls = [
        "https://kojipkgs.fedoraproject.org/compose/32/Fedora-32-20200422.0/compose/Cloud/ppc64le/images/Fedora-Cloud-Base-32-1.6.ppc64le.qcow2",
        "https://storage.googleapis.com/builddeps/dd989a078d641713c55720ba3e4320b204ade6954e2bfe4570c8058dc36e2e5d",
    ],
)

http_file(
    name = "microlivecd_image",
    sha256 = "ae449ae8c0f73b1a7e2c394bc5385e7ab01d8fc000f5b074bc8b2aaabf931eac",
    urls = [
        "https://github.com/jean-edouard/microlivecd/releases/download/0.1/microlivecd_amd64.iso",
        "https://storage.googleapis.com/builddeps/ae449ae8c0f73b1a7e2c394bc5385e7ab01d8fc000f5b074bc8b2aaabf931eac",
    ],
)

http_file(
    name = "microlivecd_image_ppc64el",
    sha256 = "eae431d68b9dc5fab422f4b90d4204cbc28c39518780c4822970a4bef42f7c7f",
    urls = [
        "https://github.com/jean-edouard/microlivecd/releases/download/0.1/microlivecd_ppc64el.iso",
        "https://storage.googleapis.com/builddeps/eae431d68b9dc5fab422f4b90d4204cbc28c39518780c4822970a4bef42f7c7f",
    ],
)

http_file(
    name = "virtio_win_image",
    sha256 = "7bf7f53e30c69a360f89abb3d2cc19cc978f533766b1b2270c2d8344edf9b3ef",
    urls = [
        "https://fedorapeople.org/groups/virt/virtio-win/direct-downloads/archive-virtio/virtio-win-0.1.171-1/virtio-win-0.1.171.iso",
        "https://storage.googleapis.com/builddeps/7bf7f53e30c69a360f89abb3d2cc19cc978f533766b1b2270c2d8344edf9b3ef",
    ],
)

load(
    "@io_bazel_rules_go//go:deps.bzl",
    "go_register_toolchains",
    "go_rules_dependencies",
)

go_rules_dependencies()

go_register_toolchains(
    go_version = "1.13.14",
    nogo = "@//:nogo_vet",
)

load("@com_github_atlassian_bazel_tools//goimports:deps.bzl", "goimports_dependencies")

goimports_dependencies()

load("@com_google_protobuf//:protobuf_deps.bzl", "protobuf_deps")

protobuf_deps()

load(
    "@bazel_gazelle//:deps.bzl",
    "gazelle_dependencies",
    "go_repository",
)

gazelle_dependencies()

load("@com_github_bazelbuild_buildtools//buildifier:deps.bzl", "buildifier_dependencies")

buildifier_dependencies()

load(
    "@bazel_tools//tools/build_defs/repo:git.bzl",
    "git_repository",
)

# Winrmcli dependencies
go_repository(
    name = "com_github_masterzen_winrmcli",
    commit = "c85a68ee8b6e3ac95af2a5fd62d2f41c9e9c5f32",
    importpath = "github.com/masterzen/winrm-cli",
)

# Winrmcp deps
go_repository(
    name = "com_github_packer_community_winrmcp",
    commit = "c76d91c1e7db27b0868c5d09e292bb540616c9a2",
    importpath = "github.com/packer-community/winrmcp",
)

go_repository(
    name = "com_github_masterzen_winrm_cli",
    commit = "6f0c57dee4569c04f64c44c335752b415e5d73a7",
    importpath = "github.com/masterzen/winrm-cli",
)

go_repository(
    name = "com_github_masterzen_winrm",
    commit = "1d17eaf15943ca3554cdebb3b1b10aaa543a0b7e",
    importpath = "github.com/masterzen/winrm",
)

go_repository(
    name = "com_github_nu7hatch_gouuid",
    commit = "179d4d0c4d8d407a32af483c2354df1d2c91e6c3",
    importpath = "github.com/nu7hatch/gouuid",
)

go_repository(
    name = "com_github_dylanmei_iso8601",
    commit = "2075bf119b58e5576c6ed9f867b8f3d17f2e54d4",
    importpath = "github.com/dylanmei/iso8601",
)

go_repository(
    name = "com_github_gofrs_uuid",
    commit = "abfe1881e60ef34074c1b8d8c63b42565c356ed6",
    importpath = "github.com/gofrs/uuid",
)

go_repository(
    name = "com_github_christrenkamp_goxpath",
    commit = "c5096ec8773dd9f554971472081ddfbb0782334e",
    importpath = "github.com/ChrisTrenkamp/goxpath",
)

go_repository(
    name = "com_github_azure_go_ntlmssp",
    commit = "4a21cbd618b459155f8b8ee7f4491cd54f5efa77",
    importpath = "github.com/Azure/go-ntlmssp",
)

go_repository(
    name = "com_github_masterzen_simplexml",
    commit = "31eea30827864c9ab643aa5a0d5b2d4988ec8409",
    importpath = "github.com/masterzen/simplexml",
)

go_repository(
    name = "org_golang_x_crypto",
    commit = "4def268fd1a49955bfb3dda92fe3db4f924f2285",
    importpath = "golang.org/x/crypto",
)

# bazel docker rules
load(
    "@io_bazel_rules_docker//container:container.bzl",
    "container_image",
    "container_pull",
)
load(
    "@io_bazel_rules_docker//repositories:repositories.bzl",
    container_repositories = "repositories",
)

container_repositories()

http_file(
    name = "go_puller_linux_ppc64le",
    executable = True,
    sha256 = "540f4d7b2a3d627d7c3190f11c4fab5f8aad48bd42a9dffb037786e26270b6bd",
    urls = [
        "https://storage.googleapis.com/builddeps/540f4d7b2a3d627d7c3190f11c4fab5f8aad48bd42a9dffb037786e26270b6bd",
    ],
)

http_file(
    name = "go_pusher_linux_ppc64le",
    executable = True,
    sha256 = "961e5a11677ab5ebf9d7ada76864ca271abcc795a6808ac2e7e98b3458b4e435",
    urls = [
        "https://storage.googleapis.com/builddeps/961e5a11677ab5ebf9d7ada76864ca271abcc795a6808ac2e7e98b3458b4e435",
    ],
)

# Pull base image fedora32
container_pull(
    name = "fedora",
    digest = "sha256:e0010fafee32e44491518e29ce640a9ab498314de6114811293b1a1ad2489791",
    registry = "index.docker.io",
    repository = "library/fedora",
    tag = "32",
)

container_pull(
    name = "fedora_ppc64le",
    digest = "sha256:38834da710c2e42dedb3182fa0fc1066e892a3e3478c55dd96ca501213c754de",
    puller_linux = "@go_puller_linux_ppc64le//file:downloaded",
    registry = "index.docker.io",
    repository = "library/fedora",
    tag = "32",
)

# Pull fedora 32 customize container-disk
container_pull(
    name = "fedora_sriov_lane",
    digest = "sha256:2d332d28863d0e415d58e335e836bd4f8a8c714e7a9d1f8f87418ef3db7c0afb",
    registry = "index.docker.io",
    repository = "kubevirt/fedora-sriov-testing",
    #tag = "32",
)

# Pull base image libvirt
container_pull(
    name = "libvirt",
    digest = "sha256:6a817da0fa85d6698e93594ef9d1d084358d62c93ed1b1237f3d147f77f92b58",
    registry = "index.docker.io",
    repository = "kubevirt/libvirt",
    #tag = "av-8.2-20200629-e049c89",
)

# TODO: Update this once we have PPC builds of the base image available
container_pull(
    name = "libvirt_ppc64le",
    digest = "sha256:NOT_AVAILABLE",  # Make sure we don't use outdated image by mistake
    puller_linux = "@go_puller_linux_ppc64le//file:downloaded",
    registry = "index.docker.io",
    repository = "kubevirt/libvirt",
)

# Pull kubevirt-testing image
container_pull(
    name = "kubevirt-testing",
    digest = "sha256:eb86f7388217bb18611c8c4e6169af3463c2a18f420314eb4d742b3d3669b16f",
    registry = "index.docker.io",
    repository = "kubevirtci/kubevirt-testing",
    #tag = "28",
)

container_pull(
    name = "kubevirt-testing_ppc64le",
    digest = "sha256:eb86f7388217bb18611c8c4e6169af3463c2a18f420314eb4d742b3d3669b16f",
    #tag = "28",
    puller_linux = "@go_puller_linux_ppc64le//file:downloaded",
    registry = "index.docker.io",
    repository = "kubevirtci/kubevirt-testing",
)

# Pull nfs-server image
container_pull(
    name = "nfs-server",
    digest = "sha256:8c1fa882dddb2885c4152e9ce632c466f4b8dce29339455e9b6bfe71f0a3d3ef",
    registry = "index.docker.io",
    repository = "kubevirtci/nfs-ganesha",  # see https://github.com/slintes/docker-nfs-ganesha
)

container_pull(
    name = "nfs-server_ppc64le",
    digest = "sha256:8c1fa882dddb2885c4152e9ce632c466f4b8dce29339455e9b6bfe71f0a3d3ef",
    puller_linux = "@go_puller_linux_ppc64le//file:downloaded",
    registry = "index.docker.io",
    repository = "kubevirtci/nfs-ganesha",  # see https://github.com/slintes/docker-nfs-ganesha
)

load(
    "@io_bazel_rules_docker//go:image.bzl",
    _go_image_repos = "repositories",
)

_go_image_repos()

http_archive(
    name = "io_bazel_rules_container_rpm",
    sha256 = "151261f1b81649de6e36f027c945722bff31176f1340682679cade2839e4b1e1",
    strip_prefix = "rules_container_rpm-0.0.5",
    urls = [
        "https://github.com/rmohr/rules_container_rpm/archive/v0.0.5.tar.gz",
        "https://storage.googleapis.com/builddeps/151261f1b81649de6e36f027c945722bff31176f1340682679cade2839e4b1e1",
    ],
)

# Get container-disk-v1alpha RPM's
http_file(
    name = "qemu-img",
    sha256 = "475b6de876914aec2187ac4858a13ae75585f5c4cb5d739c637f79a5ca6f05f9",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora/linux/releases/32/Everything/x86_64/os/Packages/q/qemu-img-4.2.0-7.fc32.x86_64.rpm",
    ],
)

http_file(
    name = "qemu-img_ppc64le",
    sha256 = "8a1b3d782d742ddca276e94dcb4821a4678aa92b9c78dfd30ce1999f0b323849",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora-secondary/releases/32/Everything/ppc64le/os/Packages/q/qemu-img-4.2.0-7.fc32.ppc64le.rpm",
    ],
)

http_file(
    name = "bzip2",
    sha256 = "b6601c8208b1fa3c41b582bd648c737798bf639da1a049efc0e78c37058280f2",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora/linux/releases/32/Everything/x86_64/os/Packages/b/bzip2-1.0.8-2.fc32.x86_64.rpm",
    ],
)

http_file(
    name = "bzip2_ppc64le",
    sha256 = "e593e694a232829765969e7270cc355d2353436cd2f950029cfa4c0549125f7f",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora/linux/releases/32/Everything/x86_64/os/Packages/b/bzip2-1.0.8-2.fc32.x86_64.rpm",
    ],
)

http_file(
    name = "capstone",
    sha256 = "40f581188b6c3d4982aa0cdfd0fdb912fdaa613a2ac615bfe5fdf26f907c8c2a",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora/linux/releases/32/Everything/x86_64/os/Packages/c/capstone-4.0.1-11.fc32.x86_64.rpm",
    ],
)

http_file(
    name = "capstone_ppc64le",
    sha256 = "0b8cdb18e2851dcc0d4e806627a4f5ac613ed33478f72282713c980688d1a22b",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora-secondary/releases/32/Everything/ppc64le/os/Packages/c/capstone-4.0.1-11.fc32.ppc64le.rpm",
    ],
)

http_file(
    name = "libaio",
    sha256 = "a410db5c56d4f39f6ea71e7d5bb6d4a2bd518015d1e34f38fbc0d7bbd4e872d4",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora/linux/releases/32/Everything/x86_64/os/Packages/l/libaio-0.3.111-7.fc32.x86_64.rpm",
    ],
)

http_file(
    name = "libaio_ppc64le",
    sha256 = "03e5a42873709ae7a6cab5fa2f5f41618b8ec03791ccb355afd57887818902d9",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora-secondary/releases/32/Everything/ppc64le/os/Packages/l/libaio-0.3.111-7.fc32.ppc64le.rpm",
    ],
)

http_file(
    name = "libstdc",
    sha256 = "be998dfbcc9ca8e3021ac4f56ed723cfa3fa1517524e89ee0b636f623abe995f",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora/linux/releases/32/Everything/x86_64/os/Packages/l/libstdc++-10.0.1-0.11.fc32.x86_64.rpm",
    ],
)

http_file(
    name = "libstdc_ppc64le",
    sha256 = "0a019186580599ebd6ddec57fb4ebc91adf5d35f770f364a330b800c215222ba",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora-secondary/releases/32/Everything/ppc64le/os/Packages/l/libstdc++-10.0.1-0.11.fc32.ppc64le.rpm",
    ],
)

http_file(
    name = "qemu-guest-agent",
    sha256 = "ee6ca269e8acf09214f2a1b1bf55b72d8177fdcfb4a70ef49a01fa0c2d998b11",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora/linux/releases/32/Everything/x86_64/os/Packages/q/qemu-guest-agent-4.2.0-7.fc32.x86_64.rpm",
    ],
)

http_file(
    name = "qemu-guest-agent_ppc64le",
    sha256 = "6212d3f37603ec702a4397d3343bade4b6bdc5d36dfe287eca2997354acbfa56",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora-secondary/releases/32/Everything/ppc64le/os/Packages/q/qemu-guest-agent-4.2.0-7.fc32.ppc64le.rpm",
    ],
)

http_file(
    name = "stress",
    sha256 = "047ed8a6297cbf06c336d9f853c2e121528638b76dcebb5453d744e6d75a96d5",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora/linux/releases/32/Everything/x86_64/os/Packages/s/stress-1.0.4-24.fc32.x86_64.rpm",
    ],
)

http_file(
    name = "stress_ppc64le",
    sha256 = "e84d0ad191bd5497d4f9eb1b3f3fb8676293e35e674b57ac336bd68bb8e82f80",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora-secondary/releases/32/Everything/ppc64le/os/Packages/s/stress-1.0.4-24.fc32.ppc64le.rpm",
    ],
)

http_file(
    name = "e2fsprogs",
    sha256 = "2fa5e252441852dae918b522a2ff3f46a5bbee4ce8936e06702bf65f57d7ff99",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora/linux/releases/32/Everything/x86_64/os/Packages/e/e2fsprogs-1.45.5-3.fc32.x86_64.rpm",
    ],
)

http_file(
    name = "e2fsprogs_ppc64le",
    sha256 = "e8772a8fab827cef27fe0781be26c2dd5cf55d0f9a8882ba20cb66712ca0d3d7",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora-secondary/releases/32/Everything/ppc64le/os/Packages/e/e2fsprogs-1.45.5-3.fc32.ppc64le.rpm",
    ],
)

http_file(
    name = "dmidecode",
    sha256 = "e40be03bd5808e640bb5fb18196499680a7b7b1d3fce47617f987baee849c0e5",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora/linux/releases/32/Everything/x86_64/os/Packages/d/dmidecode-3.2-5.fc32.x86_64.rpm",
    ],
)

http_file(
    name = "which",
    sha256 = "82e0d8f1e0dccc6d18acd04b7806350343140d9c91da7a216f93167dcf650a61",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora/linux/releases/32/Everything/x86_64/os/Packages/w/which-2.21-19.fc32.x86_64.rpm",
    ],
)

http_file(
    name = "virt-what",
    sha256 = "36f626b9f8c7fe218b893333385756681d18ffb4f888c8f14d1c1aae5e8df465",
    urls = [
        "https://dl.fedoraproject.org/pub/fedora/linux/releases/32/Everything/x86_64/os/Packages/v/virt-what-1.20-2.fc32.x86_64.rpm",
    ],
)

# some repos which are not part of go_rules anymore
go_repository(
    name = "com_github_golang_glog",
    importpath = "github.com/golang/glog",
    sum = "h1:VKtxabqXZkF25pY9ekfRL6a582T4P37/31XEstQ5p58=",
    version = "v0.0.0-20160126235308-23def4e6c14b",
)

go_repository(
    name = "org_golang_google_grpc",
    importpath = "google.golang.org/grpc",
    sum = "h1:M5a8xTlYTxwMn5ZFkwhRabsygDY5G8TYLyQDBxJNAxE=",
    version = "v1.30.0",
)

go_repository(
    name = "org_golang_x_net",
    importpath = "golang.org/x/net",
    sum = "h1:oWX7TPOiFAMXLq8o0ikBYfCJVlRHBcsciT5bXOrH628=",
    version = "v0.0.0-20190311183353-d8887717615a",
)

go_repository(
    name = "org_golang_x_text",
    importpath = "golang.org/x/text",
    sum = "h1:g61tztE5qeGQ89tm6NTjjM9VPIm088od1l6aSorWRWg=",
    version = "v0.3.0",
)

register_toolchains("//:py_toolchain")

go_repository(
    name = "org_golang_x_mod",
    build_file_generation = "on",
    build_file_proto_mode = "disable",
    importpath = "golang.org/x/mod",
    sum = "h1:RM4zey1++hCTbCVQfnWeKs9/IEsaBLA8vTkd0WVtmH4=",
    version = "v0.3.0",
)

go_repository(
    name = "org_golang_x_xerrors",
    build_file_generation = "on",
    build_file_proto_mode = "disable",
    importpath = "golang.org/x/xerrors",
    sum = "h1:go1bK/D/BFZV2I8cIQd1NKEZ+0owSTG1fDTci4IqFcE=",
    version = "v0.0.0-20200804184101-5ec99f83aff1",
)
