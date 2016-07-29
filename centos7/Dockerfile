FROM centos:7

RUN yum install -y python rpm-build git

RUN curl "https://bootstrap.pypa.io/get-pip.py" -o "get-pip.py" && python get-pip.py

RUN pip install setuptools-scm && pip install --upgrade setuptools

VOLUME /build

#COPY . /build/

ENTRYPOINT ["python", "setup.py"]

WORKDIR /build
ENV HOME=/build/

