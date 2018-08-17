CouchDB with customizable API
=============================

CouchDB 1.7.2 with rewrite function
-----------------------------------------------
This is a fork of Apache CouchDB 1.7.2 with the rewrite function that was introduced in 2.0 added.
The rewrite function allows for customizing the API of CouchDB and for creating firewalls, routers, round-robin load balancers, caching and more.
In combination with the possibility to use CouchDB as a proxy for anything else on the net – a feature that was removed in CouchDB 2.x – the rewrite function was a small, but important step forward for those that explored CouchDB to create so-called "couch apps".

As the Apache CouchDB project has discontinued the single-node 1.x branch and announced a priority to make CouchDB a pure database system, stripping it from the built-in web and application server functionality, this repo is a starting point for a new project that will emphasize these features.

The creation of forks to pursue the features of the integrated web and app server was encouraged by members of the Apache CouchDB PMC to stop a long-winded discussion about these features.

CouchDB 1.7.2 – here with the rewrite function added – is released as an unofficial version 1.7.3.

Further developments will be released in a separate repo to preserve this as repo with minimal changes to the battle-hardened official CouchDB 1.7.2.


Apache CouchDB README
=====================

Installation
------------

For a low-level guide, see:

    INSTALL

For a high-level guide to Unix-like systems, inc. Mac OS X and Ubuntu, see:

    INSTALL.Unix

For a high-level guide to Microsoft Windows, see:

    INSTALL.Windows

Follow the proper instructions to get CouchDB installed on your system.

If you're having problems, skip to the next section.

Documentation
-------------

We have documentation:

    http://docs.couchdb.org/

They include a changelog:

    http://docs.couchdb.org/en/latest/changelog.html

For troubleshooting, see:

    http://wiki.apache.org/couchdb/Troubleshooting

If you're getting a cryptic error message, see:

    http://wiki.apache.org/couchdb/Error_messages

For general help, see:

     http://couchdb.apache.org/#mailing-list
     
We also have an IRC channel:

    http://webchat.freenode.net/?channels=couchdb

The mailing lists provide a wealth of support and knowledge for you to tap into.
Feel free to drop by with your questions or discussion. See the official CouchDB
website for more information about our community resources.

Running the Testsuite
---------------------

Run the testsuite for couch.js and jquery.couch.js by browsing here:

    http://127.0.0.1:5984/_utils/spec/run.html

It should work in at least Firefox >= 3.6 with Private Browsing mode enabled.

Read more about JSpec here:

    https://github.com/liblime/jspec

When you change the specs, but your changes have no effect, manually reload
the changed spec file in the browser. When the spec that tests Erlang views
fails, make sure you have enabled Erlang views as described here:
   
       http://wiki.apache.org/couchdb/EnableErlangViews

Cryptographic Software Notice
-----------------------------

This distribution includes cryptographic software. The country in which you
currently reside may have restrictions on the import, possession, use, and/or
re-export to another country, of encryption software. BEFORE using any
encryption software, please check your country's laws, regulations and policies
concerning the import, possession, or use, and re-export of encryption software,
to see if this is permitted. See <http://www.wassenaar.org/> for more
information.

The U.S. Government Department of Commerce, Bureau of Industry and Security
(BIS), has classified this software as Export Commodity Control Number (ECCN)
5D002.C.1, which includes information security software using or performing
cryptographic functions with asymmetric algorithms. The form and manner of this
Apache Software Foundation distribution makes it eligible for export under the
License Exception ENC Technology Software Unrestricted (TSU) exception (see the
BIS Export Administration Regulations, Section 740.13) for both object code and
source code.

The following provides more details on the included cryptographic software:

CouchDB includes a HTTP client (ibrowse) with SSL functionality.
