### Example 1: Update the accountEnabled property of a device

```powershellImport-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	accountEnabled = $false
}

Update-MgBetaDevice -DeviceId $deviceId -BodyParameter $params
```
This example shows how to use the Update-MgBetaDevice Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

### Example 2:  Write extensionAttributes on a device

```powershellImport-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	extensionAttributes = @{
		extensionAttribute1 = "BYOD-Device"
	}
}

Update-MgBetaDevice -DeviceId $deviceId -BodyParameter $params
```
This example shows how to use the Update-MgBetaDevice Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

