# Vagrant Hadoop cluster

## Architecture

One master (`hadoop-manager`) and 3 slaves (`hadoop-nodeXX`).

## Instructions

Once the cluster is up, do installation using the [Cloudera Manager](http://www.cloudera.com/content/cloudera/en/products/cloudera-manager.html).

    $ git clone git://github.com/sgomezvillamor/vagrant-hadoop-cluster.git
    $ cd vagrant-hadoop-cluster
    $ vagrant up
    $ vagrant ssh manager
    [vagrant@hadoop-manager ~]$ wget http://archive.cloudera.com/cm4/installer/latest/cloudera-manager-installer.bin
    [vagrant@hadoop-manager ~]$ chmod +x cloudera-manager-installer.bin
    [vagrant@hadoop-manager ~]$ sudo ./cloudera-manager-installer.bin

After that, go to http://192.168.56.2:7180
