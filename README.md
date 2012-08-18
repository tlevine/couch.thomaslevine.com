couch.thomaslevine.com
======================

Install couch

    apt-get install couchdb
    
Configure it

    echo 'bind_address=0.0.0.0' >> /etc/couchdb/local.ini
    echo 'port = 5984' >>  /etc/couchdb/local.ini

Kill [all remnants](http://serverfault.com/questions/79453/why-cant-i-access-my-couchdb-instance-externally-on-ubuntu-9-04-server)
of it to reload the configuration. Do this manually, or just reboot.