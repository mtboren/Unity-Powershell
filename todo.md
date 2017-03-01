todo:
- add cmdlets to handle HostLUN objects, the place from where HLU info can be had, and where HLUs can be set
- add something to update PowerShell window titlebar with Unity connected-session info, as a convenience

done:
- updated `New-UnityLun`, `New-UnityVMwareLun` to actually enable compression by default (help said that they did, but they did not)
- updated several `Get-Unity*` cmdlets to have proper "fields=..." values for request URI -- viable values seem to have changed in the API version that apparently has come out since module author worked on these items, and the given `Get-Unity*` cmdlets were all failing due to invalid field values being specified by default:  `Get-UnityLUNResource`, `Get-UnityFastCache`, `Get-UnityFilesystem`, `Get-UnityPool`, `Get-UnityStorageResource`
