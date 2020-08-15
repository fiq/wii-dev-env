# wii DevKit Dev Environment

I've thrown this together for the kids to mess around with. It puts some layers
around the devkitpro container.

# To Start 
``dc up``

# Set up DevCode

1. Copy a starter project from workspace into build. Eg ``cp -r workspace/examples/wii/graphics/gx/triangle builds``
1. Start the container with ``docker-compose up``
1. The container will loop and continuously run make in the folder
1. See ``builds/wiidev.failure`` for errors from the build
1. See ``builds/wiidev.output`` for other output 

# To sin and work directly on the Container (_If you want_)

You can start and control tmux sessions on the container:
``docker-compose exec wiidev -it tmux``

