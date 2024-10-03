# eBPF

开发和运行所需要的开发工具：

将 eBPF 程序编译成字节码的 LLVM；
C 语言程序编译工具 make；
最流行的 eBPF 工具集 BCC 和它依赖的内核头文件；
与内核代码仓库实时同步的 libbpf；
同样是内核代码提供的 eBPF 程序管理工具 bpftool

## BCC 安装

必要的开发工具和开发库
sudo apt-get install -y  make clang llvm libelf-dev libbpf-dev libbpfcc-dev linux-tools-$(uname -r) linux-headers-$(uname -r)
