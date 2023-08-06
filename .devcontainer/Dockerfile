# See here for image contents: https://github.com/sarisia/mikanos-docker
ARG VARIANT=latest
FROM ghcr.io/sarisia/mikanos:${VARIANT}

# [Optional] Uncomment this section to install additional OS packages.
# RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
#     && apt-get -y install --no-install-recommends <your-package-here>
# create a symlink to MikanLoaderPkg in my repository
RUN cd /home/${USERNAME}/edk2 &&  ln -s /workspaces/mikanos/MikanLoaderPkg ./

# create a symlink to my Conf/
RUN cd /home/${USERNAME}/edk2 && rm -rf ./Conf && ln -s /workspaces/mikanos/edk2/Conf ./
