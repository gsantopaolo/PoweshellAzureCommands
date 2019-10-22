# PoweshellAzureCommands
Login to Azure
=
`Connect-AzureRmAccount`

Switch subscrition
=
`Set-AzureRmContext -SubscriptionId "YOUR SUBSCRITION ID"`

Enable AcceleratedNetworking on VM
=

```
$nic = Get-AzureRmNetworkInterface -ResourceGroupName "YOUR RESOURCE NAME" -Name "NETWORK INTERFACE NAME"
$nic.EnableAcceleratedNetworking = $true
Set-AzureRmNetworkInterface
```
