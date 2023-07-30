FROM stepkun/vulcanexus:iron-full 

# set timezone
ENV TZ="Europe/Berlin"

# ** [Optional] Uncomment this section to install additional packages. **
#
# ENV DEBIAN_FRONTEND=noninteractive
# RUN apt-get update \
#    && apt-get -y install --no-install-recommends <your-package-list-here> \
#    #
#    # Clean up
#    && apt-get autoremove -y \
#    && apt-get clean -y \
#    && rm -rf /var/lib/apt/lists/*
# ENV DEBIAN_FRONTEND=dialog

# Set up auto-source of workspace for ros user
ARG WORKSPACE
ARG USER
RUN echo "if [ -f ${WORKSPACE}/install/setup.bash ]; then source ${WORKSPACE}/install/setup.bash; fi" >> /home/$USER/.bashrc \
  && echo "export ROS_LOCALHOST_ONLY=0" >> /home/$USER/.bashrc

WORKDIR $WORKSPACE
USER $USER
# default CMD to startup container
CMD /bin/sh -c "while sleep 1000; do :; done"
