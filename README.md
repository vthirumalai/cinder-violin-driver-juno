# cinder-violin-driver-juno
Openstack Cinder FC driver for the violin 7300 FSP platform
cinder-violin-driver-icehouse
*** WARNING: Alpha release. Use at your own risk! ***

6000 Series All-Flash Array Volume Driver V1.5.0 for OpenStack Cinder Icehouse Release.

This repository contains the latest open-source release of Violin Memory's python drivers and client communication libraries for use with Openstack Cinder's block storage services.

It is maintained externally for 3rd party developers, testers, and users and may be periodically updated in the future.

Overview

The Volume Driver package for OpenStack Juno from Violin Memory adds block-storage service support for Violin V7300/V7700 series Flash Storage Platforms. The package is implemented as a storage "plug-in" using the standard Cinder storage driver API, and facilitates the creation, attachment, and management of volumes (LUNs) between a Flash Array and different host servers.

All Cinder volume features required for the OpenStack Icehouse release are supported, including volume, snapshot, and clone operations. The 3.0.0 driver package release can be used with any OpenStack Juno deployment V7300/V7700 Series arrays running V7.5.4 (or newer) with either FibreChannel connectivity.

This plug-in software is available as an installable tarball. Use at your own risk. Software and support for existing Violin Memory customers is available from the Violin Memory Support portal at www.violinmemory.com/support.

Setup

Download a zip file of this repository (using the "Download ZIP" button to the right). Unzip the file on the machine(s) running Cinder's volume service (cinder-volume).

Recursively copy the cinder directory to the same directory as your cinder code installation.

Examples:

For devstack: 'cp -r cinder /opt/stack/cinder'

For ubuntu: 'cp -r cinder /usr/local/lib/python2.7/dist-packages/cinder'

Follow your system documentation to enable FibreChannel and configure your HBAs.

Configure cinder to use one of the Violin drivers (see below).

Restart cinder-volume.


For more details on the Setup and Installation documents, please read the accompanying documents.
