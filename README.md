# docker-python-setuptools
a docker container that has python setuptools for building python things

## how to use this

   * install docker
   * `docker pull treyduskin/python-setuptools`
   * `cd` to your project with a `setup.py`
   * `$ docker run -v $PWD:/build treyduskin/python-setuptools <your setup.py command>`

## environment specifics

in some OS environments, the pythonpath is different than what the build environment
might be.  this can cause problems for building RPMs or DEBs.  to handle that, there are
tagged docker images that provide the same python-setuptools interface but based
on a different OS:

   * `latest`: ubuntu:trusty (./Dockerfile)
   * `centos7`: centos:7 (./centos7/Dockerfile)
 
