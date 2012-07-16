SDShare test suite
==================

This project provides a test suite for
[SDShare](http://www.sdshare.org) server implementations. It verifies
compliance with the Atom 1.0 spec, and the SDShare 2012-07-10 draft.

Running the test suite
----------------------

The system property `org.sdshare.serveraddress` must 
be set to an IRI where the SDShare server runs (i.e. http://localhost:8888/).

Example:

    java -Dorg.sdshare.serveraddress=http://localhost:8888 -jar sdshare-tests.jar

Picky server tests
------------------

The system property `org.sdshare.pickyservertests` is used to enable/disable
picky server tests. `true` enables the tests (enabled by default), `false` disables
them.

Example:

    java -Dorg.sdshare.serveraddress=http://localhost:8888 -Dorg.sdshare.pickyservertests=false -jar sdshare-tests.jar

