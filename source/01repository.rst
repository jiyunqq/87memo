01repository
=====================================

#. centos 7 repository

   .. code-block:: bash

    wget -O /etc/yum.repos.d/CentOS-Base.repo http://mirrors.aliyun.com/repo/Centos-7.repo
    curl -o /etc/yum.repos.d/CentOS-Base.repo http://mirrors.aliyun.com/repo/Centos-7.repo

#. docker 镜像源

   .. code-block:: bash

    cat << EOF > /etc/docker/daemon.json
    {
      "registry-mirrors": [
        "https://dockerhub.icu"
      ]
    }
    EOF
    systemctl restart docker.service

