# Part 5: Adding an Existing RHEL VM to Satellite

[Tutorial Menu](https://github.com/pslucas0212/RedHat-Satellite-VM-Provisioning-to-vSphere-Tutorial)  

## Registering an Exsiting RHEL VM to Satellite

For simplicity of the example we will use the Operations Derpartment Organization and moline operation along with 

In this tutorial we will add an existing RHEL VM to Satellite for content management.  

If you don't already have an operating system defined in the host section we will need to do that first.  On the left side navibation bar chose Hosts -> Operating Systems.

![Host -> Operating Systems](/images/sat83.png)

On the Operating Systems page click the blud Create Operating System button. 

![Blue Operating System button](/images/sat84.png)

On the Operating Systems > Create Operating Systems page fill in or chose options from the following table, and click the blue Submit button.  We will only be filling in information on the Operating System tab and accept the default settings for any other tabs on this page.  

Name | Choice
---- | ------
Name* | RedHat
Major Version* | 8
Minor Version | 4
Family | Red Hat
Architecture | x86_64

![Define Operating System](/images/sat85.png)

Next go to the left side navibation bar chose Hosts -> Content Hosts.

![Hosts -> Content Hosts](/images/sat86.png)

On the Content Hosts page clock the Register Content Host button.

![Register Content Host](/images/sat87.png)

On the Content Host Registration button we will click the blue Register Host link and follow the new process for registering hosts.

![Blue Register Hosts link](/images/sat88.png)

On the Registrations > Register host page fill in or chose options from the following table, and click the blue Submit button.

Name | Choice
---- | ------
Host Group | hg-
Operating System | RedHat 8.4
Capsule | sat01.example.com
Activation Keys | ak-ops-rhel8-prem-server
