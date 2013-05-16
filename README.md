Rundeck hybrid login module
===========================
Overview
--------
This login module provides the possibility for a user to be authenticated via LDAP and to be authorized (get mapped to a Rundeck role) via the *.properties file.

Prerequisites
-------------
Assuming Rundeck 1.4.2+ is installed.
Also assuming, that Rundeck launcher is being started with the `--skipinstall` option to prevent re-writing the contents of `$RDECK_BASE/server/exp/webapp` on each startup.

Build
-----
Use `Ant` to build the module. The result of the build will be available under `build` directory.

Installation
------------
Stop the Rundeck server: <br/>
`rundeckd stop` <br/>
Copy the library: <br/>
`cp rundeck-hybrid-login-ext-<version>.jar $RDECK_BASE/server/exp/webapp/WEB-INF/lib` <br/>
Start the Rundeck server: <br/>
`rundeckd start` <br/>
