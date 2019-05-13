# HPC-cluster-build
## 测试搭建
### KVM虚拟机安装
#### 环境准备

    cat /etc/redhat-release
    ifconfig
    getenforce #检查SElinux是否启动
    关闭SElinux
    setenforce 0 #临时关闭
    #安装相关软件包
    yum install qemu-kvm libvirt virt-install virt-manager bridge-utils
    service libvirtd start
    

