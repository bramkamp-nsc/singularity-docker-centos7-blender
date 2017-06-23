BootStrap: docker
From: centos:centos7

%post
yum -y update && yum -y upgrade
yum -y install bzip2 freetype mesa-libGLU libXi libXrender mesa-dri-drivers
    curl http://download.blender.org/release/Blender2.78/blender-2.78c-linux-glibc219-x86_64.tar.bz2 | tar -C /opt -xjvf -
# specific to my setup
mkdir -p /local-storage /mnt/beegfs /baycells/home /baycells/scratch /c6/shared /c6/eb /local/gensoft2 /c6/shared/rpm /Bis/Scratch2 /mnt/beegfs

%runscript
PATH=/opt/blender-2.78c-linux-glibc219-x86_64/:${PATH}
export PATH
/opt/blender-2.78c-linux-glibc219-x86_64/blender "$@"

