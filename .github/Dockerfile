FROM registry.fedoraproject.org/fedora
RUN dnf install -y make golang krb5-devel && dnf clean all
RUN mkdir /src
WORKDIR /src
COPY . /src/
