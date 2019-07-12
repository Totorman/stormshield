# Stormshield Network Security VM with 2 network interfaces

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FTotorman%2Fstormshield%2Ftemplate.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a><a href="http://armviz.io/#/?load=https://raw.githubusercontent.com/Totorman/stormshield/template.json" target="_blank">
  <img src="http://armviz.io/visualizebutton.png"/>
</a>

This Azure Resource Manager template deploys a SNS VM with 2 network interfaces in an existing VNET.


* The virtual network has a public subnet facing Internet and a private subnet for servers
* A route table is created to route trafic from the private network through the SNS appliance

<img src="img/topo-2nics.png" alt="network topology">


## Next configuration steps:

* Setup Filtering and NAT masquerading for the Private subnet on the SNS appliance
* Deploy servers in the private subnet
* Configure NAT redirection to publish services

