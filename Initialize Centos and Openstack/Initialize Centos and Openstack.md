


# Initialize Centos and Openstack



I Installed ***Centos 9 stream*** and ***Openstack Zed***



# For opentsack installion



First i read through some doucment asna dused devstack as i thought it was i easy methods and waited for the installtion to finish and it ***Failed 😭***

I thought my system was the error i did stop the Networkmanger the firewall too still was in issue .Later i found packtsack is made for RHEL and Centos so why not use that and i Installed ***Failed again 😭*** and when I restared the system I couldn't connect the system as Network Manger does everyhting for Centos 9 and network -scripts is depricated



I went throught the net to see why is this error and so this post saying do a fresh strat of installtion it might work so I formated the system again and used packstack but this time was reading RDO project throughly and so that



> They haven't mention anything about disabling/stoping firewalld and NetworkManger for Centos 9 stream so I thought why not try it without disabling/stoping it



So I Installed Packstack and Ran the setp up and it was a ***SUCCESS YIPPI KI-YAY***

  ![sd](https://tenor.com/view/brooklyn-nine-nine-charles-boyle-yippie-kayak-other-buckets-joe-lo-truglio-gif-22232816.gif)





Later on I had an issue was powercut in SL when this powercut happens my system will stop imediatlety because my UPS is not working so ineede to find some way to stop that from happening so i craeted some cronjobs so that server shutdowns before time it self and this way I can save my **HOME LAB SEVER** and also i instlled the frivers for my processor in centos



And also i had another issue i said before that I didn't stop firewalld but later on it made an issue after reboot I couldn't see the dashboard so I needed to make a another script to stop firewalld when booting up i could have **disabled it** ,But i want to keep it na dfind aswya to use the firewall and aslo run opentsakc smoothly without shuttimng down any service that's all I did for now will tell u later on what I'm doing next