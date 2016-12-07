
TDM pit container
=================

This container needs both elasticsearch and fedora's activemq broker running. They can be linked to this container, for example, like:

    $ docker run --name pit --link es:es --link fedora:fedora -d test/pit \
        run --index-host es --broker-host fedora
