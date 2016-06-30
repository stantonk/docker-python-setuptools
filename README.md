# docker-python-setuptools
a docker container that has python setuptools for building python things

## how to use this

   * install docker
   * `docker pull treyduskin/python-setuptools`
   * `cd` to your project with a `setup.py`
   * `$ docker run -v $PWD:/build treyduskin/python-setuptools <your setup.py command, like bdist_rpm>`
 
