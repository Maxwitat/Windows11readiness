Custom MECM  report to display Windows 11 readiness information

If you plan to migrate to Windows 11, you will probably want to determine which machines fulfill the requirements for an upgrade. If you are using MECM, you can find this information for single machines in the Resource Explorer.
 
The Resource Explorer information is based on the view v_GS_UPGRADE_EXPERIENCE_INDICATORS which is fed by the hardware inventory. The hardware inventory gets it from the registry (HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\AppCompatFlags\TargetVersionUpgradeExperienceIndicators). These settings are set by the Microsoft Compatibility Appraiser which runs daily as scheduled task.
If your environment is tenant attached, you’ll find the same information in MEM Endpoint analytics. For devices managed by MECM, the ConfigMgr service connector will upload this information every hour. 

In case your environment is not cloud attached, this report will give you the Windows 11 readiness information by extending the MECM standard reports. 



