couch.thomaslevine.com
======================

Install couch

    apt-get install couchdb
    
Configure it

    echo 'bind_address=0.0.0.0' >> /etc/couchdb/local.ini

Kill [all remnants](http://serverfault.com/questions/79453/why-cant-i-access-my-couchdb-instance-externally-on-ubuntu-9-04-server)
of it to reload the configuration. Do this manually, or just reboot.

The couch server is currently the same as the rewrite server,
but I plan on getting rid of the rewrite server and switching
the couch port to 80.