pash
====

# Pentaho Analysis Shell

Pash is an abbreviation for Pentaho Analysis Shell.

Pash is an interactive XML/A query tool written in html/javascript/css.

With pash you can:

* connect to a XML for Analysis (XML/A) server
* retrieve metadata about the available cubes, dimensions, measures etc.
* execute MDX queries

# Running Pash

Pash was originally written for the Pentaho BI server, but can be used with any XML/A server.

## On Pentaho

Pash is available through the Pentaho marketplace. From within the server, open the marketplace, find the entry for Pentaho Analysis Shell, and click install. (Server restart required).

If you like you can also manually deploy Pash. To do that, simply download the bin/pash.zip package and unzip into pentaho-solutions/system beneath your Pentaho BI Server home directory.

After the install, you can open Pash by clicking the "Pentaho Analysis Shell" menu item in the "Tools" menu.
To open pash outside of the Pentaho user console, point your browser to http://localhost:8080/pentaho/contents/pash/html/index.html

(Modify hostname, portnumber and "pentaho" accordingly if you changed those when configuring your pentaho server)

## On Jasper Reports Server

Download the bin/pash.zip package and unzip into apache-tomcate/webapps beneath your jasper reports server home directory.

You can start pash by pointing your browser to http://localhost:8080/pash/html/index.html

(Modify hostname and portnumber accordingly as necessary)

## On icCube

Download the bin/pash.zip package and unzip into the web directory beneath your icCube home directory.

You can start pash by pointing your browser to http://localhost:8282/pash/html/index.html

(Modify hostname and portnumber accordingly as necessary)

## On a standalone mondrian XML/A server

Download the bin/pash.zip package and unzip into whatever is the webapps directory of your server.

You can start pash by pointing your browser to http://yourserver:yourport/pash/html/index.html

## On IIS / MS Analysis services

This scenario assumes you already set up XML/A access to your MS Analysis instance.
(If you need instructions to do that, please refer to https://msdn.microsoft.com/en-us/library/gg492140(v=sql.110).aspx)

Download the bin/pash.zip package and unzip to someplace beneath the wwwroot (Normally in C:\inetpub\) your IIS server.
Let's say you put it in C:\inetpub\wwwroot\pash

You can now start pash by navigating your browser to

http://yourserver/pash/html/index.html

However, this assumes you setup your XML/A endpoint at

http://yourserver/olap/msmdpump.dll

If you setup your XML/A endpoint under a different URL, you need to specify it via the XmlaUrl query parameter.

http://yourserver/pash/html/index.html?XmlaUrl=http://yourserver/...your path...
