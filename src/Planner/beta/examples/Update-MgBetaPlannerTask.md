### Example 1: Code snippet

```powershellImport-Module Microsoft.Graph.Beta.Planner

$params = @{
	assignments = @{
		"fbab97d0-4932-4511-b675-204639209557" = @{
			"@odata.type" = "#microsoft.graph.plannerAssignment"
			orderHint = "N9917 U2883!"
		}
	}
	appliedCategories = @{
		category3 = $true
		category4 = $false
	}
	recurrence = @{
		schedule = @{
			pattern = @{
				type = "daily"
				interval = 3
			}
			patternStartDateTime = [System.DateTime]::Parse("2022-02-22T02:10:33Z")
		}
	}
}

Update-MgBetaPlannerTask -PlannerTaskId $plannerTaskId -BodyParameter $params-If-Match W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
This example shows how to use the Update-MgBetaPlannerTask Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

