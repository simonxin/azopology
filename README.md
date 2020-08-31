# aztopologyviz

PowerShell Module that can generate a topology diagram to Visualize Azure Network Topology and ARM templates (WIP). It has capabilities to insert appropriate Azure Icons depending upon the type of the Azure Resource you have in your Resource Group, like Virtual Machine, Virtual Network, Subnet etc.

# Azure Resource Network Topology Visualization

### Working with Single Azure Resource Group

```PowerShell
Import-Module Aztopviz

Get-AzrgVizualization -ResourceGroups 'test-resource-group' -ShowGraph -OutputFormat png -Verbose
```

### Working with Multiple Azure Resource Group

```PowerShell
$ResourceGroups = 'test-resource-group', 'demo-resource-group'
Get-AzrgVizualization -ResourceGroups $ResourceGroups  -ShowGraph -OutputFormat png -Verbose
```

# Does this looks like Network Watcher -> Monitor -> Topology feature? 
