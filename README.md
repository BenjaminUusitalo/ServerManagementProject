# ServerManagementProject

Mini Project for Tero Karvinen's Server Management ICT4TN022-3014 - 2021 course

In this project I will attempt to make a salt state, which I can use to install, run and manage some useful everyday programs. 

With this, if I ever install a new machine for which I want these programs up and running, this state will do so with essentially a single command.

## Starting out

To start, Install Salt Master-Slave.

For Master

```
master$ sudo apt-get update
master$ sudo apt-get -y install salt-master
```

For Slave

```
slave$ sudo apt-get update
slave$ sudo apt-get -y install salt-minion
```

Next to create sls files for wanted programs

On Master create a new directory, I did /srv/salt/yourdir

Within the directory create a new init.sls file.

Inside will be the configurations, in my case this was the Apache 2 file, which looked like this:

![Image](./SC/1.png)



 
