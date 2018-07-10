FROM bartfeenstra/ola:0.1

USER root

RUN apt-get update && apt-get install sudo udev -y
RUN usermod -aG dialout olad
RUN usermod -aG plugdev olad

RUN cp /etc/udev/rules.d/ftdi.rules /etc/udev/rules.d/10-ftdi.rules

USER olad

