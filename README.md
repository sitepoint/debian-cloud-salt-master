debian-cloud-salt-master
========================

Salt master installer plugin for Andsen's
[build-debian-cloud](https://github.com/andsens/build-debian-cloud) fork.

## Usage

To install the plugin clone the [git
repository](https://github.com/sitepoint/debian-cloud-salt-master)
and pass the plugin to build-debian-cloud:

    ./build-debian-cloud (ec2 | gce) \
        --plugin <path_to>/debian-cloud-salt-master/salt-master

A repository that contains the deb packages must be specified via the
$SALT_REPO environment variable, or it will default to:

    deb http://ftp.debian.org/debian/ ${distribution}-backports main
