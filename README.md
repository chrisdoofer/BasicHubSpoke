# Hub and Spoke Topology Sandbox

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fchrisdoofer%2Fbasichubspoke%2Fmain%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fchrisdoofer%2Fbasichubspoke%2Fmain%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

This template creates a basic hub-and-spoke topology setup. It creates a Hub VNet with subnets DMZ, Management, Shared and Gateway (optionally), with two Spoke VNets, development and production, containing a workload subnet each. It also deploys a Windows Jump-Host on the Management subnet of the HUB, and establishes VNet peerings between the Hub and the two spokes. 

Note that if you choose to deploy the VPN gateway, it may take up to 45 minutes to complete.
