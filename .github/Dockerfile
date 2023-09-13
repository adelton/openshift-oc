FROM registry.fedoraproject.org/fedora
RUN dnf install -y 'dnf-command(builddep)' rpm-build && dnf clean all
RUN mkdir /src
WORKDIR /src
COPY . /src/
RUN dnf builddep -y oc.spec && dnf clean all
