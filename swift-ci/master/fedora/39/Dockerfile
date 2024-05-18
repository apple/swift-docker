FROM fedora:39

RUN groupadd -g 998 build-user && \
    useradd -m -r -u 998 -g build-user build-user

RUN yum install -y \
  libcurl-devel       \
  libedit-devel       \
  libicu-devel        \
  sqlite-devel        \
  libuuid-devel       \
  libxml2-devel       \
  python3             \
  python3-devel       \
  python3-distro      \
  python3-setuptools  \
  python3-six         \
  rsync               \
  swig                \
  clang               \
  perl-podlators      \
  which               \
  diffutils

USER build-user

WORKDIR /home/build-user