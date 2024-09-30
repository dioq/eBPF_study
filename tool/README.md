# compile tool

wget https://aka.pw/bpf-ecli -O ecli && chmod +x ./ecli
./ecli -h

wget https://github.com/eunomia-bpf/eunomia-bpf/releases/latest/download/ecc && chmod +x ./ecc
./ecc -h

## 使用 ecc 编译程序

./ecc test.c

## 然后使用 ecli 运行编译后的程序

sudo ./ecli run package.json

## 查看 /sys/kernel/debug/tracing/trace_pipe 文件来查看 eBPF 程序的输出

sudo cat /sys/kernel/debug/tracing/trace_pipe | grep "BPF triggered sys_enter_write"
