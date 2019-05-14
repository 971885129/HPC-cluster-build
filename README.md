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
    #创建网桥
    
    #创建安装磁盘
    mkdir -p /media/sdb2/linux/kvm1
    qemu-img create -f qcow2 /var/linux/images/centos74.img 20G
        Formatting '/media/sdb2/linux/kvm1/centos74.img', fmt=qcow2 size=21474836480 encryption=off cluster_size=65536 

    

