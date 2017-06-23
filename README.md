# singularity-docker-centos7-blender
blender singularity container on CentOS-7

although blender page seems to required glibc >= 2.19, CentOS-7 glibc-2.17-157.el7_3.4.x86_64 (as of 2017-06-23) seems to be ok.
```
singularity run shub://truatpasteurdotfr/singularity-docker-centos7-blender
or ln -s truatpasteurdotfr-singularity-docker-centos7-blender,img ~/bin/blender
```
