#Remove-SPOUserFromGroup
Removes a user from a group
##Syntax
```powershell
Remove-SPOUserFromGroup -LoginName <String>
                        -Identity <GroupPipeBind>
                        [-Web <WebPipeBind>]
```


##Parameters
Parameter|Type|Required|Description
---------|----|--------|-----------
|Identity|GroupPipeBind|True|A group object, an ID or a name of a group|
|LoginName|String|True|A valid login name of a user (user@company.com)|
|Web|WebPipeBind|False|The web to apply the command to. Omit this parameter to use the current web.|
##Examples

###Example 1
```powershell
PS:> Remove-SPOUserFromGroup -LoginName user@company.com -GroupName 'Marketing Site Members'
```

