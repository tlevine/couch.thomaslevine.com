couch.thomaslevine.com
======================

Install couch

    apt-get install couchdb
    
Configure it

    # Listen on all ports.
    echo 'bind_address=0.0.0.0' >> /etc/couchdb/local.ini
    
    # Redirect port 80 to 5984.
    iptables -t nat -A PREROUTING -p tcp --dport 80 -j REDIRECT --to-ports 5984

Kill [all remnants](http://serverfault.com/questions/79453/why-cant-i-access-my-couchdb-instance-externally-on-ubuntu-9-04-server)
of it to reload the configuration. Do this manually, or just reboot.