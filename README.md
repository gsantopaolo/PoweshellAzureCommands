# PoweshellAzureCommands
Login to Azure
=
`Connect-AzureRmAccount`

Switch subscrition
=
`Set-AzureRmContext -SubscriptionId "YOUR SUBSCRITION ID"`

Enable AcceleratedNetworking on VM
=
Only some VM instances support Accelerated Networking, for a detailed list refer to [Microsoft official documentation](https://docs.microsoft.com/en-us/azure/virtual-network/create-vm-accelerated-networking-cli#supported-vm-instances) 
```
$nic = Get-AzureRmNetworkInterface -ResourceGroupName "YOUR RESOURCE NAME" -Name "NETWORK INTERFACE NAME"
$nic.EnableAcceleratedNetworking = $true
Set-AzureRmNetworkInterface
```
