BootStrap: docker
From: nvidia/cuda:8.0-cudnn6-runtime-ubuntu16.04

################################################################################
%labels
################################################################################
MAINTAINER Wolfgang Resch
VERSION v3

################################################################################
%environment
################################################################################
export PATH=/usr/local/sbin:/usr/sbin:/sbin/bin:/usr/bin:/usr/local/bin:/usr/local/cuda/bin

################################################################################
%post
################################################################################

deb http://downloads.skewed.de/apt/xenial xenial universe
deb-src http://downloads.skewed.de/apt/xenial xenial universe
apt-get update
apt-get install python-graph-tool
apt-get clean

###
### destination for NIH HPC bind mounts
###

mkdir /gpfs /spin1 /gs2 /gs3 /gs4 /gs5 /gs6 /gs7 /gs8 /data /scratch /fdb /lscratch
