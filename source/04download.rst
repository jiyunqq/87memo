04download 常用下载
================================================

#. 通用下载

   ====================  =======================================================================
   nvidia 驱动下载        https://www.nvidia.cn/Download/index.aspx?lang=cn
   mellanox ib 驱动	      https://network.nvidia.com/products/infiniband-drivers/linux/mlnx_ofed/
   cuda 下载	            https://developer.nvidia.com/cuda-downloads
   anaconda	              https://www.anaconda.com/download/success
   miniconda	            https://conda.io/projects/conda/en/latest/index.html
   NVIDIA HPC SDK	        https://developer.nvidia.com/hpc-sdk-downloads
   cmake	                https://cmake.org/download/
   ====================  =======================================================================

#. centos 7.9 专用下载

   - cuda 11.6.0 https://developer.download.nvidia.com/compute/cuda/11.6.0/local_installers/cuda_11.6.0_510.39.01_linux.run
   - cuda 11.6.2 https://developer.download.nvidia.com/compute/cuda/11.6.2/local_installers/cuda_11.6.2_510.47.03_linux.run
   - cuda 11.8.0 https://developer.download.nvidia.com/compute/cuda/11.8.0/local_installers/cuda_11.8.0_520.61.05_linux.run
   - cuda 10.1.2 https://developer.download.nvidia.com/compute/cuda/10.1/Prod/local_installers/cuda_10.1.243_418.87.00_linux.run
   - cuda 12.1.1 https://developer.download.nvidia.com/compute/cuda/12.1.1/local_installers/cuda_12.1.1_530.30.02_linux.run

#. centos 8.5 专用下载

   - centos 8.5 系统镜像 https://mirrors.cloud.tencent.com/centos/8.5.2111/isos/x86_64/CentOS-8.5.2111-x86_64-dvd1.iso
   - cuda 11.6.2 https://developer.download.nvidia.com/compute/cuda/11.6.2/local_installers/cuda_11.6.2_510.47.03_linux.run
   - cuda 12.1.1 https://developer.download.nvidia.com/compute/cuda/12.1.1/local_installers/cuda_12.1.1_530.30.02_linux.run

#. nvidia 显卡驱动下载

   - 3080ti/3090 (CUDA: 12.2): https://cn.download.nvidia.com/XFree86/Linux-x86_64/535.104.05/NVIDIA-Linux-x86_64-535.104.05.run
   - 4090D (cuda: 12.4): https://cn.download.nvidia.com/XFree86/Linux-x86_64/550.76/NVIDIA-Linux-x86_64-550.76.run

#. 其它通用下载

   - centos 7.9 系统镜像 https://mirrors.aliyun.com/centos/7.9.2009/isos/x86_64/CentOS-7-x86_64-DVD-2009.iso
   - oneapi basekit https://registrationcenter-download.intel.com/akdlm/irc_nas/18673/l_BaseKit_p_2022.2.0.262_offline.sh
   - oneapi hpckit https://registrationcenter-download.intel.com/akdlm/irc_nas/18679/l_HPCKit_p_2022.2.0.191_offline.sh
   - oneapi 百度网盘下载链接: https://pan.baidu.com/s/1LkRvy98VJ2e04VB4qczYjQ?pwd=lxkt 提取码: lxkt
   - openssl 下载: https://www.openssl.org/source/old/1.0.1/openssl-1.0.1e.tar.gz
   - openssl 下载: https://www.openssl.org/source/old/1.0.2/openssl-1.0.2u.tar.gz
   - FusionOS 兼容 openssl: compat-openssl10-1.0.2o-3.fos22.u1.x86_64.rpm
   - pwmat python 环境离线版本: `pwmat_license.tgz <https://pan.baidu.com/s/17ctUAQNlnUWx_Xg6dnpSkQ?pwd=lxkt%E6%8F%90%E5%8F%96%E7%A0%81%EF%BC%9Alxkt>`_
   - mstation 一体机安装包链接: https://pan.baidu.com/s/1axqSIxPa2KB0ZtXEXXZ4EQ?pwd=lxkt 提取码: lxkt
   - xcat-core: https://xcat.org/files/xcat/xcat-core/2.16.x_Linux/xcat-core/xcat-core-2.16.5-linux.tar.bz2
   - xcat-dep: https://xcat.org/files/xcat/xcat-dep/2.x_Linux/xcat-dep-2.16.5-linux.tar.bz2
   - centos 7 改root密码: https://jiyunqq.github.io/soft/single.html

#. 提权漏洞补丁

   更新补丁 ::

    yum install http://mirrors.aliyun.com/centos/7/updates/x86_64/Packages/polkit-0.112-26.el7_9.1.x86_64.rpm

   centos 6.10 ::

    yum install https://mirrors.tuna.tsinghua.edu.cn/centos-vault/centos/6.10/updates/x86_64/Packages/polkit-0.96-11.el6_10.1.x86_64.rpm

   centos 8.5 ::

    wget https://mirrors.tuna.tsinghua.edu.cn/centos-vault/centos/8-stream/BaseOS/x86_64/os/Packages/polkit-0.115-15.el8.x86_64.rpm
    wget https://mirrors.tuna.tsinghua.edu.cn/centos-vault/centos/8-stream/BaseOS/x86_64/os/Packages/polkit-libs-0.115-15.el8.x86_64.rpm
