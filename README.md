# Autoscaling-Heat-Openstack
Autoscaling with Ceilometer and Heat


# How it works
Heat-engine will create one instance , then if an alarm is triggred, Heat will launch a second one.
Thresholds can be customized.


## Getting start

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

```
$ git clone https://github.com/YassineFadhlaoui/Autoscaling-Heat.git
$ cd Autoscaling-Heat
```

# Running the tests

First Of all , you must change the path of cirros.yaml in env.yaml and change networks names in fedora.yaml to suit you needs 
Now you are ready to launch the stack, to do so , issue the following command:

```
$ heat stack-create mystack -f scale.yaml -e env.yaml  
```

# Requirments

* Openstack installed and running
* ceilometer installed and running correctly
* Heat installed (make sure that heat-api-cfn is installed)
* Neutron installed
* Glance installed
* Nova of course

# Author

*Yassine Fadhlaoui* - **Initial work** - [Yassine Fadhlaoui](https://github.com/YassineFadhlaoui)

# License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/YassineFadhlaoui/Autoscaling-Heat-Openstack/blob/master/LICENSE) file for details
