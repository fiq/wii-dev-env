FROM devkitpro/devkitppc
RUN apt update
RUN apt-get install --yes tmux 
RUN apt-get install --yes vim
RUN apt-get install --yes wget
RUN apt-get install --yes mc
RUN apt-get install --yes locales
RUN apt-get install --yes locales-all
RUN dpkg-reconfigure locales 
RUN tmux new -s wiidev -d
#RUN mkdir -p /opt/src/sdl
#WORKDIR /opt/src/sdl
#RUN cd /opt/src/sdl
#RUN make install
WORKDIR /builds
CMD watch -n 30 make 2>/builds/wiidev.failures 1>/builds/wiidev.output
