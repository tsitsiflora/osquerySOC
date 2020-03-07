# osquerySOC
A security operations centre developed using osquery and the ELK stack

Make use of the documentation
- https://osquery.readthedocs.io/en/latest


1. Installing osquery
```
$ export OSQUERY_KEY=1484120AC4E9F8A1A577AEEE97A80C63C9D8B80B
$ sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys $OSQUERY_KEY
$ sudo add-apt-repository 'deb [arch=amd64] https://pkg.osquery.io/deb deb main'
$ sudo apt-get update
$ sudo apt-get install osquery
```


After installing, the default packages create the following structure
```
/etc/osquery/
/usr/share/osquery/osquery.example.conf
/usr/share/osquery/lenses/{*}.aug
/usr/share/osquery/packs/{*}.conf
/var/log/osquery/
/usr/lib/osquery/
/usr/bin/osqueryctl
/usr/bin/osqueryd
/usr/bin/osqueryi
```

2. Activating osqueryd
```
$ sudo service osqueryd start
$ sudo systemctl enable osqueryd
$ sudo systemctl start osqueryd
```

3. Configurations

An example configuration file: https://gist.github.com/anand1996aditya/3a6ead64fe97c9529eeb76a518234f0f


