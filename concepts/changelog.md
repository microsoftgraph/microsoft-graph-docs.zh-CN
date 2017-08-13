# <a name="changelog-for-microsoft-graph"></a>Microsoft Graph 更改日志

此更改日志涵盖了 Microsoft Graph 变更，包括 v1.0 和 beta 终结点 Microsoft Graph API。  

有关 Microsoft Graph API 已知问题的详细信息，请参阅[已知问题](known_issues.md)。

## <a name="august-2017"></a>2017 年 8 月

### <a name="onenote"></a>OneNote

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
| 添加项 | v1.0 和 Beta | 向 **site** 添加了 [onenote](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onenote.md) 导航属性。  |
| 添加项 | Beta | 添加了用于复制操作的目标 *siteCollectionId* 和目标 *siteId* 参数。例如：[CopyNotebook](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/notebook_copynotebook.md)。 |


## <a name="july-2017"></a>2017 年 7 月

### <a name="group-settings"></a>组设置

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
| 添加项     | v1.0       | 添加了组设置支持。<br/>新资源类型：[groupSetting](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/groupsetting.md)、[groupSettingTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/groupsettingtemplate.md)、[settingValue](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/settingvalue.md) 和 [settingTemplateValue](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/settingtemplatevalue.md) |
| 更改       | v1.0       | 将属性 **classification** 和导航属性**settings** 添加到[组](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/group.md) |

### <a name="intune-apis"></a>Intune API

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|Beta|在 [iosMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_iosmobileappconfiguration) 上添加了 [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_apps_iosmobileappconfiguration_assign.md) 操作 |
|添加项|Beta|在 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) 上添加了 [syncDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_devices_manageddevice_syncdevice.md) 操作 |
|更改|Beta|向 [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) 实体添加了 **appsInstallAllowList**、**appsLaunchBlockList** 和 **appsHideList** 属性|
|更改|Beta|向 [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) 实体添加了 **disableAppEncryptionIfDeviceEncryptionIsEnabled** 属性|
|更改|Beta|向 [defaultManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) 实体添加了 **disableAppEncryptionIfDeviceEncryptionIsEnabled** 属性|
|更改|Beta|向 [deviceComplianceDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus) 实体添加了 **complianceGracePeriodExpirationDateTime** 属性|
|更改|Beta|向 [deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) 实体添加了 **complianceGracePeriodExpirationDateTime** 属性|
|更改|Beta|向 [deviceConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus) 实体添加了 **complianceGracePeriodExpirationDateTime** 属性|
|更改|Beta|向 [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) 实体添加了 **subscriptions** 属性|
|更改|Beta|向 [deviceManagementExchangeConnector](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_devicemanagementexchangeconnector) 实体添加了 **version** 属性|
|更改|Beta|向 [iosUpdateConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdateconfiguration) 实体添加了 **utcTimeOffsetInMinutes** 属性|
|更改|Beta|向 [iosUpdateDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdatedevicestatus) 实体添加了 **complianceGracePeriodExpirationDateTime** 属性|
|更改|Beta|向 [macOSWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoswificonfiguration) 实体添加了 **preSharedKey** 属性|
|更改|Beta|向 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) 实体添加了 **phoneNumber**、**androidSecurityPatchLevel** 和 **userDisplayName** 属性|
|更改|Beta|向 [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus) 实体添加了 **userName**、**deviceModel**、**platform** 和 **complianceGracePeriodExpirationDateTime** 属性|
|更改|Beta|向 [mobileAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus) 实体添加了 **userPrincipalName** 属性|
|更改|Beta|向 [onPremisesConditionalAccessSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_onpremisesconditionalaccesssettings) 实体添加了 **overrideDefaultRule** 属性|
|更改|Beta|向 [userAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_userappinstallstatus) 实体添加了 **userPrincipalName** 属性|
|更改|Beta|向 [windows10TeamGeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10teamgeneralconfiguration) 实体添加了 **connectAppBlockAutoLaunch**、**deviceAccountBlockExchangeServices**、**deviceAccountEmailAddress**、**deviceAccountExchangeServerAddress**、**deviceAccountRequirePasswordRotation**、**deviceAccountSessionInitiationProtocolAddress**、**settingsBlockMyMeetingsAndFiles**、**settingsBlockSessionResume**、**settingsBlockSigninSuggestions**、**settingsDefaultVolume**、**settingsScreenTimeoutInMinutes**、**settingsSessionTimeoutInMinutes** 和 **settingsSleepTimeoutInMinutes** 属性|
|更改|Beta|向 [defaultManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) 实体添加了 **deploymentSummary** 导航属性|
|更改|Beta|向 [deviceCompliancePolicySettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate) 复杂类型添加了 **settingName**、**userId**、**userName**、**userEmail** 和 **currentValue** 属性|
|更改|Beta|将 **settingName**、**userId**、**userName**、**userEmail** 和 **currentValue** 属性添加到了 [deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) 复杂类型中|
|更改|Beta|向 [deviceOperatingSystemSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devices_deviceoperatingsystemsummary) 复杂类型添加了 **unknownCount** 属性|



## <a name="june-2017"></a>2017 年 6 月

### <a name="project-rome"></a>Project Rome

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|Beta|添加了以下资源和 API：<br/>[活动](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/projectrome_activity)<br/>[创建或替换活动](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/projectrome_put_activity)<br/>[删除活动](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/projectrome_delete_activity)<br/>[历史记录项](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/projectrome_historyitem)<br/>[创建或替换历史记录项](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/projectrome_put_historyitem)<br/>[删除历史记录项](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/projectrome_delete_historyitem)|

### <a name="outlook-calendar"></a>Outlook 日历

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|v1.0|将以下 4 个 [calendar](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/calendar)属性升级到 v1.0：**canEdit**、**canShare**、**canViewPrivateItems** 和 **owner**。|


### <a name="intune-apis"></a>Intune API

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|Beta|添加的新实体：<br/>[defaultDeviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_defaultdevicecompliancepolicy)<br/>[deviceConfigurationUserStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuserstatesummary)<br/>[deviceManagementScriptDeviceState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptdevicestate)<br/>[deviceManagementScriptRunSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptrunsummary)<br/>[deviceManagementScriptUserState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptuserstate)<br/>[iosUpdateDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdatedevicestatus)<br/>[windowsManagedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanageddevice)<br/>[windowsManagementAppHealthState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapphealthstate)<br/>[windowsManagementAppHealthSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapphealthsummary)<br/>|
|添加项|Beta|新增了复杂类型：<br/>[bitLockerFixedDrivePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerfixeddrivepolicy)<br/>[bitLockerRecoveryOptions](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerrecoveryoptions)<br/>[bitLockerRemovableDrivePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerremovabledrivepolicy)<br/>[deleteUserFromSharedAppleDeviceActionResult](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_deleteuserfromsharedappledeviceactionresult)<br/>[iosNetworkUsageRule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnetworkusagerule)<br/>|
|删除|Beta|删除了以下实体：<br/>**deviceManagementScriptState**<br/>|
|删除|Beta|在[用户](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_user)上删除了 wipeByDeviceTag 操作 |
|更改|Beta|向 [androidEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidenterprisewificonfiguration) 实体添加了 **innerAuthenticationProtocolForEapTtls**、**innerAuthenticationProtocolForPeap** 和 **outerIdentityPrivacyTemporaryValue** 属性|
|更改|Beta|从 [androidEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidenterprisewificonfiguration) 实体删除了 **nonEapAuthenticationMethodForEapTtls**、**nonEapAuthenticationMethodForPeap** 和 **enableOuterIdentityPrivacy** 属性|
|更改|Beta|向 [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) 实体添加了 **deployedAppCount** 属性|
|更改|Beta|从 [complianceSettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/complianceSettingStateSummary) 实体删除了 **instanceDisplayName** 和 **settingPlatform** 属性|
|更改|Beta|向 [defaultManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) 实体添加了 **deployedAppCount** 属性|
|更改|Beta|向 [deviceCompliancePolicyGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicygroupassignment) 实体添加了 **excludeGroup** 属性|
|更改|Beta|从 [deviceCompliancePolicySettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary) 实体删除了 **instanceDisplayName** 和 **settingPlatform** 属性|
|更改|Beta|从 [deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) 实体删除了 **devicePlatform** 属性|
|更改|Beta|向 [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) 实体添加了 **assignmentStatus**、**assignmentProgress** 和 **assignmentErrorMessage** 属性|
|更改|Beta|向 [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) 实体添加了 **intuneBrand** 属性|
|更改|Beta|向 [deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript) 实体添加了 **enforceSignatureCheck** 和 **fileName** 属性|
|更改|Beta|向 [iosEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosenterprisewificonfiguration) 实体添加了 **innerAuthenticationProtocolForEapTtls** 和 **outerIdentityPrivacyTemporaryValue** 属性|
|更改|Beta|从 [iosEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosenterprisewificonfiguration) 实体删除了 **nonEapAuthenticationMethodForEapTtls** 和 **enableOuterIdentityPrivacy** 属性|
|更改|Beta|向 [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) 实体添加了 **classroomAppForceUnpromptedScreenObservation**、**keyboardBlockDictation**、**networkUsageRules** 和 **wiFiConnectOnlyToConfiguredNetworks** 属性|
|更改|Beta|向 [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) 实体添加了 **deployedAppCount** 属性|
|更改|Beta|向 [iosWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswificonfiguration) 实体添加了 **preSharedKey** 属性|
|更改|Beta|向 [macOSEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosenterprisewificonfiguration) 实体添加了 **innerAuthenticationProtocolForEapTtls** 和 **outerIdentityPrivacyTemporaryValue** 属性|
|更改|Beta|从 [macOSEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosenterprisewificonfiguration) 实体删除了 **nonEapAuthenticationMethodForEapTtls** 和 **enableOuterIdentityPrivacy** 属性|
|更改|Beta|从 [managedAppPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy) 实体删除了 **lastModifiedTime** 和 **deployedAppCount** 属性|
|更改|Beta|向 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) 实体添加了 **serialNumber** 属性|
|更改|Beta|从 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) 实体删除了 **managementAgents** 属性|
|更改|Beta|向 [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) 实体添加了 **deployedAppCount** 属性|
|更改|Beta|向 [windows10EndpointProtectionConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration) 实体添加了 **bitLockerFixedDrivePolicy** 和 **bitLockerRemovableDrivePolicy** 属性|
|更改|Beta|向 [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) 实体添加了 **enterpriseCloudPrintDiscoveryEndPoint**、**enterpriseCloudPrintOAuthAuthority**、**enterpriseCloudPrintOAuthClientIdentifier**、**enterpriseCloudPrintResourceIdentifier**、**enterpriseCloudPrintDiscoveryMaxLimit**、**enterpriseCloudPrintMopriaDiscoveryResourceIdentifier**、**edgeBlockAddressBarDropdown**、**edgeBlockCompatibilityList**、**edgeClearBrowsingDataOnExit**、**edgeAllowStartPagesModification**、**edgeDisableFirstRunPage**、**edgeBlockLiveTileDataCollection** 和 **edgeSyncFavoritesWithInternetExplorer** 属性|
|更改|Beta|向 [windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp) 实体添加了 **availableVersion** 属性|
|更改|Beta|从 [windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp) 实体删除了 **onboardingStatus**、**deployedVersion** 和 **lastModifiedTime** 属性|
|更改|Beta|向 [windowsStoreForBusinessApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessapp) 实体添加了 **packageIdentityName** 属性|
|更改|Beta|向 [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) 实体添加了 **mobileAppIdentifierDeployments** 和 **deploymentSummary** 导航属性|
|更改|Beta|向 [defaultManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) 实体添加了 **mobileAppIdentifierDeployments** 导航属性|
|更改|Beta|向 [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) 实体添加了 **deviceConfigurationUserStateSummaries** 和 **iosUpdateStatuses** 导航属性|
|更改|Beta|从 [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) 实体删除了 **complianceSettingStateSummaries** 导航属性|
|更改|Beta|向 [deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript) 实体添加了 **runSummary**、**deviceRunStates** 和 **userRunStates** 导航属性|
|更改|Beta|从 [deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript) 实体删除了 **runStates** 导航属性|
|更改|Beta|向 [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) 实体添加了 **mobileAppIdentifierDeployments** 和 **deploymentSummary** 导航属性|
|更改|Beta|从 [managedAppPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy) 实体删除了 **mobileAppIdentifierDeployments** 和 **deploymentSummary** 导航属性|
|更改|Beta|向 [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) 实体添加了 **mobileAppIdentifierDeployments** 和 **deploymentSummary** 导航属性|
|更改|Beta|向 [windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp) 实体添加了 **healthSummary** 和 **healthStates** 导航属性|
|更改|Beta|向 [appInstallationFailure](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure) 复杂类型添加了 **applicationId**、**appName**、**platformId**、**userFailures** 和 **deviceFailures** 属性|
|更改|Beta|向 [bitLockerSystemDrivePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockersystemdrivepolicy) 复杂类型添加了 **encryptionMethod**、**startupAuthenticationRequired**、**startupAuthenticationBlockWithoutTpmChip**、**startupAuthenticationTpmUsage**、**startupAuthenticationTpmPinUsage**、**startupAuthenticationTpmKeyUsage**、**startupAuthenticationTpmPinAndKeyUsage**、**recoveryOptions** 和 **prebootRecoveryEnableMessageAndUrl** 属性|
|更改|Beta|从 [deviceCompliancePolicySettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate) 复杂类型删除了 **settingName**、**userId**、**userName**、**userEmail** 和 **currentValue** 属性|
|更改|Beta|从 [deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) 复杂类型删除了 **settingName**、**userId**、**userName**、**userEmail** 和 **currentValue** 属性|
|更改|Beta|向 [deviceManagementSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) 复杂类型添加了 **windowsCommercialId** 和 **windowsCommercialIdLastModifiedTime** 属性|
|更改|Beta|向 [vpnServer](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_vpnserver) 复杂类型添加了 **address** 属性|


## <a name="may-2017"></a>2017 年 5 月

### <a name="application-api-changes"></a>应用程序 API 更改

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|更改|Beta| 应用程序 API 更新。这是第一组更改，其中包括[应用程序](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/application)实体的属性重命名和重构。<br/>**新实体：**[api](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/api])、[informationalUrl](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/informationalUrl)、[installedClient](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/installedclient)、[permissionScope](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/permissionscope)、[preauthorizedApplication](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/preauthorizedapplication)、[Web](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/web)。<br/>**删除的属性：**addIns、appRoles、availableToOtherOrganizations、knownClientApplications、oauth2AllowUrlPathMatching、recordConsentConditions。<br/>**重命名的属性：**appId 重命名为 id，identifierUris 重命名为 applicationAliases，availableToOtherTenants 重命名为 orgRestrictions，mainLogo 重命名为 logo，oauth2Permissions 重命名为 publishedPermissionsScopes，publicClient 重命名为 allowPublicClient，replyUrls 重命名为 redirectUrls。<br/>**新属性：**tags。 |

### <a name="remove-deprecated-planner-api"></a>删除已弃用的 Planner API
|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:-------------|
|删除|Beta|删除了以下实体：<br/>**task**<br/>**plan**<br/>**bucket**<br/>**taskDetails**<br/>**planDetails**<br/>**taskBoardTaskFormat**<br/>**planTaskBoard**|

### <a name="project-rome"></a>Project Rome

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:-------------|
|添加项|Beta|添加了对 Project Rome 的支持，包括[获取设备列表](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_list_devices)、[发送命令到设备](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/send_device_command)和[查看命令状态](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/get_device_command_status)。|
|添加项|Beta|增加了对用户[活动](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/projectrome_activity)和 [historyItems](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/projectrome_historyitem) 的支持，其中包括 [upsert 活动](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/projectrome_put_activity)和 [upsert historyItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/projectrome_put_historyitem)。|

### <a name="administrative-units-property-changes"></a>管理单元属性更改

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
| 更改        | Beta       | 已将 [scopedRoleMembership](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/scopedrolemembership) 实体的 roleMemberInfo 属性类型更改为 [identity](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/identity) |
| 更改        | Beta       | 已将 [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/user) 实体的导航属性 scopedAdministratorOf 更改为 scopedRoleMemberOf |
| 更改        | Beta       | 已将 [administrativeUnit](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/administrativeunit) 实体的导航属性 scopedAdministrators 更改为 scopedRoleMembers |
| 更改        | Beta       | 已将 [directoryRole](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/directoryrole) 实体的导航属性 scopedAdministrators 更改为 scopedMembers |

### <a name="add-users-and-groups-webhook-support-in-preview"></a>在预览中添加用户和组 Webhook 支持

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
| 更改        | Beta       | 添加了用户和组的 [Webhooks](https://developer.microsoft.com/graph/docs/api-reference/beta/resources/webhooks) 支持

### <a name="add-delta-query-to-v10"></a>向 v1.0 添加 delta 查询

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
| 添加项      | v1.0       | 向 V1.0 添加 delta 函数支持。添加到以下实体，以执行 [delta 查询](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_overview)：<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>有关示例，请参阅以下文章：<br/>[获取组的增量更改](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_groups)<br/>[获取文件夹中邮件的增量更改](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_messages)<br/>[获取用户的增量更改](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_users)|
| 更改        | Beta       | 将其他可选查询筛选功能（按 id）添加到 [users](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_delta) 和 [groups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/group_delta)。 |

### <a name="added-user-resource-support-for-deleted-items"></a>添加了对已删除项目的用户资源支持

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
| 添加项      | Beta       | 添加了对[还原并永久删除用户](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/directory)的支持。 |

### <a name="added-onpremisesprovisioningerror"></a>添加了 OnPremisesProvisioningError

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
| 添加项      | beta       | 新实体：[OnPremisesProvisioningError](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/onpremisesprovisioningerror) |
| 更改        | beta       | 向 [user](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/user)、[group](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/group) 和 [orgcontact](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/orgcontact) 添加了 OnPremisesProvisioningError 属性。 |

### <a name="added-deleteddatetime-property"></a>添加了 deletedDateTime 属性

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|更改|beta|向 [user](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/user) 实体添加了 deletedDateTime 属性。
|更改|beta|向 [group](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/group) 实体添加了 deletedDateTime 属性。
|更改|beta|向 [application](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/application) 实体添加了 deletedDateTime 属性。

### <a name="added-domain-operations-to-v10"></a>向 v1.0 添加了域操作

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|v1.0|在 [domains](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domain) 上添加了操作<br/>新实体：</br>[domain](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domain)<br/>[domainDnsRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domaindnsrecord)<br/>[domainDnsCnameRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsCnameRecord)<br/>[domainDnsMxRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsMxRecord)<br/>[domainDnsSrvRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsSrvRecord)<br/>[domainDnsTxtRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsTxtRecord)<br/>[domainDnsUnavailableRecord](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/domainDnsUnavailableRecord)<br/>新操作：</br>[verify](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/api/domain_verify) |

### <a name="added-contracts-to-v10"></a>向 v1.0 添加了合同

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|v1.0|新实体：</br>[contract](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/contract) |

### <a name="added-licensedetails-to-v10"></a>向 v1.0 添加了 licenseDetails

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|v1.0|新实体：</br>[licenseDetails](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/licensedetails) |
|更改  |v1.0|针对 [users](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/user) 的新 [licensedetails](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/api/user_list_licensedetails) 导航属性 |


### <a name="drive-api"></a>驱动器 API

|**更改类型**|**版本**|**说明**|
|:--------------|:----------|:--------------|
| 添加项 | v1.0 | 添加了 **baseItem** 资源类型，其中包含 **driveItem** 中的基本属性。
| 添加项 | v1.0 和 Beta | 向 **thumbnail** 添加了 **sourceItemId** 属性。 <br/> 向 **sharepointIds** 添加了 **siteUrl** 属性。 <br/> 向 **shared** 添加了 **sharedBy** 和 **sharedDateTime** 属性。 <br/> 向 **remoteItem** 添加了 **shared** 属性。 <br/> 向 **drive** 和 **itemReference** 添加了 **sharepointIds** 属性。 <br/> 向 **fileSystemInfo** 添加了 **lastAccessedDateTime**。 <br/> 向 **sharedDriveItem** 添加了 **driveItem** 和 **site** 导航属性。 <br/> 向 **baseItem** 添加了 **parentReference** 属性。
| 更改 | v1.0 和 Beta | 已将 **driveItem** 和 **sharedDriveItem** 更改为从 **baseItem** 继承。 <br/> 已将 **identity** 标记为“开放类型”。
| 更改 | Beta | 向 **sharingLink** 添加了 **configuratorUrl** 和 **WebHtml** 属性。 <br/> 向 **folder** 资源类型添加了 **folderView** 资源类型和 **view** 属性。 <br/> 向 **driveItem** 添加了 **listItem** 导航属性。 <br/> 向 **drive** 添加了 **list** 导航属性。


### <a name="extensions-open-extensions"></a>扩展（开放扩展）

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|v1.0| 支持下列资源中的 [openTypeExtension](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/opentypeextension)：[device](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/device)、[group](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/group)、[organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/organization)、[user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)。 |
|添加项|v1.0 和 beta|当用户使用个人 Microsoft 帐户登录时，在下列资源中支持开放扩展：event、post、group、message、contact 和 user。（除了这些资源，还有 device、group、organization 和 user，它们会在用户使用工作或学校帐户登录时支持开放扩展。）|
|添加项|v1.0 和 beta|支持 `$expand` 在下列资源中[获取开放扩展](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/opentypeextension_get)：[device](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/device)、[group](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/group)、[organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/organization)、[post](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/post)、[user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)。|
|添加项|Beta|支持 `$expand` 在 [administrativeUnit](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/administrativeunit) 中[获取开放扩展](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/opentypeextension_get)。|


### <a name="extensions-schema-extensions"></a>扩展（架构扩展） 

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|v1.0|新资源 [schemaExtension](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/schemaextension) 和用于管理以下资源的扩展定义的 CRUD 方法：[contact](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/contact)、[device](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/device)、[event](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/event)、[group](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/group)、[message](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/message)、[organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/organization)、[post](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/post)、[user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)。请注意，对 [administrativeUnit](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/administrativeunit) 的支持仍和以前一样仅限于测试版本。|
|添加项|v1.0|下列资源中的现有 POST、GET 和 PATCH方法 - [contact](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/contact)、[device](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/device)、[event](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/event)、[group](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/group)、[message](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/message)、[organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/organization)、[post](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/post)、[user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) - 现在支持添加、获取、更新或删除作为架构扩展存储在相应资源实例中的自定义数据。|
|添加项|v1.0 和 beta| 现在，你可以使用 `$filter` 来查找具有与特定扩展属性值相匹配的属性的资源实例，如扩展名。有关详细信息，请参阅此[示例](https://devx.microsoft-tst.com/en-us/graph/docs/concepts/extensibility_schema_groups#5-get-a-group-and-its-extension-data)。 |
|更改|v1.0 和 beta| [删除架构扩展定义](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/schemaextension_delete)不再会影响访问基于此定义添加的自定义数据。 |
|更改|v1.0 和 beta| 现在可以将架构扩展复杂类型设为 null，以便将架构扩展从资源实例中删除。 |


### <a name="group"></a>组

|**更改类型**|**版本**|**说明**|
|:--------------|:----------|:--------------|
| 添加项 | v1.0 和 beta | 向 **group** 添加了 **drives** 和 **sites** 导航属性。

### <a name="insights-apis"></a>见解 API

|**更改类型**|**版本**|**说明**| 
|:-------------|:-----------|:--------------|
|添加项|Beta|添加了 [Shared API](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_shared)。<br />新资源：<br />[sharingDetail](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_sharingdetail) <br />[insightIdentity](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_insightidentity) <br />
|添加项|Beta|添加了 [Used API](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_used)。<br />新资源：<br />[usageDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_usagedetails) <br />
|更改|Beta|以下资源中的新 **Type** 属性：<br />[resourceVisualization](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/insights_resourcevisualization)。 <br />
|删除项|Beta|删除了以下实体：<br/>**workingWith**<br/>**trendingAround**<br/>|

### <a name="intune-apis"></a>Intune API

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|Beta|添加的新实体：<br/>[androidForWorkMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidforworkmobileappconfiguration)<br/>[cartToClassAssociation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_carttoclassassociation)<br/>[deviceCompliancePolicySettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary)<br/>[eBookInstallSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_ebookinstallsummary)<br/>[eBookVppGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_ebookvppgroupassignment)<br/>[iosUpdateConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdateconfiguration)<br/>[remoteAssistancePartner](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner)<br/>[windows10EndpointProtectionConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration)<br/>[windowsDeviceMalwareState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsdevicemalwarestate)<br/>[windowsInformationProtectionAppLearningSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_wip_windowsinformationprotectionapplearningsummary)<br/>[windowsMalwareInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsmalwareinformation)<br/>[windowsProtectionState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsprotectionstate)<br/>|
|添加项|Beta|添加的新复杂类型：<br/>[androidPermissionAction](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidpermissionaction)<br/>[bitLockerSystemDrivePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockersystemdrivepolicy)<br/>[defenderDetectedMalwareActions](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_defenderdetectedmalwareactions)<br/>[settingSource](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_settingsource)<br/>|
|添加项|Beta|在 [managedEBook](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_managedebook) 上添加了 [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_books_managedebook_assign) 操作 |
|添加项|Beta|在 [remoteAssistancePartner](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner) 上添加了 [beginOnboarding](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_remoteassistance_remoteassistancepartner_beginonboarding) 操作 |
|添加项|Beta|在 [remoteAssistancePartner](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner) 上添加了 [disconnect](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_remoteassistance_remoteassistancepartner_disconnect) 操作 |
|删除|Beta|删除了以下实体：<br/>**outlookTask**<br/>**outlookTaskFolder**<br/>**outlookTaskGroup**<br/>**outlookUser**<br/>**windowsManagementAppHealthState**<br/>|
|删除|Beta|删除了以下复杂类型：<br/>**applePushNotificationCertificateSetting**<br/>**eventCreationOptions**<br/>|
|更改|Beta|向 [androidForWorkGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgeneraldeviceconfiguration) 实体添加了 **workProfilePasswordBlockFingerprintUnlock**、**workProfilePasswordBlockTrustAgents**、**workProfilePasswordExpirationDays**、**workProfilePasswordMinimumLength**、**workProfilePasswordMinutesOfInactivityBeforeScreenTimeout**、**workProfilePasswordPreviousPasswordBlockCount**、**workProfilePasswordSignInFailureCountBeforeFactoryReset**、**workProfilePasswordRequiredType** 和 **workProfileRequirePassword** 属性|
|更改|Beta|向 [androidForWorkPkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkpkcscertificateprofile) 实体添加了 **subjectAlternativeNameFormatString** 属性|
|更改|Beta|向 [androidForWorkScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile) 实体添加了 **subjectNameFormatString** 和 **subjectAlternativeNameFormatString** 属性|
|更改|Beta|向 [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) 实体添加了 **kioskModeManagedApps** 属性|
|更改|Beta|从 [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) 实体删除了 **kioskModeManagedAppId** 属性|
|更改|Beta|向 [androidPkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidpkcscertificateprofile) 实体添加了 **subjectAlternativeNameFormatString** 属性|
|更改|Beta|向 [androidScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidscepcertificateprofile) 实体添加了 **subjectNameFormatString** 和 **subjectAlternativeNameFormatString** 属性|
|更改|Beta|从 [calendar](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/calendar) 实体删除了 **hexColor** 属性|
|更改|Beta|将 **setting** 和 **platformType** 属性添加到了 [complianceSettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_compliancesettingstatesummary) 实体中|
|更改|Beta|从 [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) 实体删除了 **windowsManagementAppEnabled** 属性|
|更改|Beta|向 [deviceComplianceDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus) 实体添加了 **userName**、**deviceModel** 和 **platform** 属性|
|更改|Beta|向 [deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) 实体添加了 **userPrincipalName** 和 **deviceModel** 属性|
|更改|Beta|将 **platformType**、**setting**、**userId** 和 **userEmail** 属性添加到了 [deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) 实体中|
|更改|Beta|将 **inGracePeriodCount** 属性添加到了 [deviceCompliancePolicyDeviceStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary) 实体中|
|更改|Beta|向 [deviceConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus) 实体添加了 **userName**、**deviceModel** 和 **platform** 属性|
|更改|Beta|从 [event](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/event) 实体删除了 **creationOptions** 属性|
|更改|Beta|从 [eventMessage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/eventMessage) 实体删除了 **isDelegated** 属性|
|更改|Beta|从 [group](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/group) 实体删除了 **unseenConversationsCount** 和 **unseenMessagesCount** 属性|
|更改|Beta|向 [iosMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_iosmobileappconfiguration) 实体添加了 **settingXml** 和 **settings** 属性|
|更改|Beta|向 [iosPkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iospkcscertificateprofile) 实体添加了 **subjectAlternativeNameFormatString** 属性|
|更改|Beta|向 [iosScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosscepcertificateprofile) 实体添加了 **subjectAlternativeNameFormatString** 属性|
|更改|Beta|向 [macOSCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscompliancepolicy) 实体添加了 **systemIntegrityProtectionEnabled** 属性|
|更改|Beta|向 [macOSScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosscepcertificateprofile) 实体添加了 **subjectAlternativeNameFormatString** 属性|
|更改|Beta|将 **complianceGracePeriodExpirationDateTime**、**userPrincipalName** 和 **imei** 属性添加到了 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) 实体中|
|更改|Beta|从 [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration) 实体删除了 **settingXml** 和 **settings** 属性|
|更改|Beta|向 [officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp) 实体添加了 **useSharedComputerActivation**、**updateChannel**、**officePlatformArchitecture** 和 **localesToInstall** 属性|
|更改|Beta|从 [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_organization) 实体删除了 **applePushNotificationCertificateSetting** 属性|
|更改|Beta|更改了 [post](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/post) 实体上的以下属性：<br/>将 **sender** 从可选更改为必需<br/>|
|更改|Beta|向 [softwareUpdateStatusSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_softwareupdatestatussummary) 实体添加了 **compliantUserCount**、**nonCompliantUserCount**、**remediatedUserCount**、**errorUserCount**、**unknownUserCount**、**conflictUserCount**和 **notApplicableUserCount** 属性|
|更改|Beta|向 [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) 实体添加了 **bluetoothAllowedServices**、**bluetoothBlockPrePairing**、**cellularData**、**defenderDetectedMalwareActions**、**defenderPotentiallyUnwantedAppAction**、**lockScreenAllowTimeoutConfiguration**、**lockScreenBlockCortana**、**lockScreenBlockToastNotifications**、**lockScreenTimeoutInSeconds**、**passwordBlockSimple**、**privacyAutoAcceptPairingAndConsentPrompts**、**privacyBlockInputPersonalization**、**startMenuHideChangeAccountSettings**、**startMenuHideHibernate**、**startMenuHideLock**、**startMenuHideShutDown**、**startMenuHideSignOut**、**startMenuHideSleep**、**startMenuHideSwitchAccount**、**settingsBlockAppsPage**、**settingsBlockGamingPage**、**windowsSpotlightBlockConsumerSpecificFeatures**、**windowsSpotlightBlocked**、**windowsSpotlightBlockOnActionCenter**、**windowsSpotlightBlockTailoredExperiences**、**windowsSpotlightBlockThirdPartyNotifications**、**windowsSpotlightBlockWelcomeExperience**、**windowsSpotlightBlockWindowsTips**、**windowsSpotlightConfigureOnLockScreen** 和 **connectedDevicesServiceBlocked** 属性。|
|更改|Beta|从 [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) 实体删除了 **automaticUpdateMode**、**automaticUpdateSchedule**、**automaticUpdateTime**、**prereleaseFeatures**、**experienceBlockWindowsSpotlight**、**experienceBlockWindowsTips** 和 **experienceBlockConsumerSpecificFeatures** 属性。|
|更改|Beta|向 [windows10PkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10pkcscertificateprofile) 实体添加了 **subjectAlternativeNameFormatString** 属性|
|更改|Beta|向 [windows81SCEPCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81scepcertificateprofile) 实体添加了 **subjectNameFormatString** 和 **subjectAlternativeNameFormatString** 属性|
|更改|Beta|向 [windowsInformationProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) 实体添加了 **indexingEncryptedStoresOrItemsBlocked** 和 **smbAutoEncryptedFileExtensions** 属性|
|更改|Beta|更改了 [windowsInformationProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) 实体上的以下属性：<br/>将 **rightsManagementServicesTemplateId** 从必需更改为可选<br/>|
|更改|Beta|更改了 [windowsMobileMSI](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi) 实体上的以下属性：<br/>将 **productCode** 从必需更改为可选<br/>|
|更改|Beta|向 [windowsPhone81SCEPCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81scepcertificateprofile) 实体添加了 **subjectNameFormatString** 和 **subjectAlternativeNameFormatString** 属性|
|更改|Beta|向 [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) 实体添加了 **mobileAppConfigurations** 导航属性|
|更改|Beta|将 **cartToClassAssociations**、**deviceCompliancePolicySettingStateSummaries**、**remoteAssistancePartners**、**windowsInformationProtectionAppLearningSummaries** 和**windowsMalwareInformation** 导航属性添加到了 [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) 实体中|
|更改|Beta|向 [eBookGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_ebookgroupassignment) 实体添加了 **eBook** 导航属性|
|更改|Beta|向 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) 实体添加了 **windowsProtectionState** 导航属性|
|更改|Beta|向 [managedEBook](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_managedebook) 实体添加了 **installSummary** 导航属性|
|更改|Beta|从 [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_user) 实体删除了 **outlook** 导航属性|
|更改|Beta|从 [windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapp) 实体删除了 **healthStates** 导航属性|
|更改|Beta|向 [defaultDeviceEnrollmentRestrictions](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_defaultdeviceenrollmentrestrictions) 复杂类型添加了 **androidForWorkRestrictions** 属性|
|更改|Beta|向 [deviceCompliancePolicySettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate) 复杂类型添加了 **userPrincipalName** 和 **sources** 属性|
|更改|Beta|向 [deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) 复杂类型添加了 **userPrincipalName** 和 **sources** 属性|
|更改|Beta|将 **settingName**、**userId**、**userName**、**userEmail** 和 **currentValue** 属性添加到了 [deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) 复杂类型中|
|更改|Beta|从 [mailboxSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/mailboxSettings) 复杂类型删除了 **archiveFolder** 属性|


### <a name="outlook-calendar"></a>Outlook 日历

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|v1.0 和 beta|对于 **findMeetingTimes**，添加了新的枚举值**无限制**，你可以将其指定为 **activityDomain** 属性并作为 **timeConstraint** 参数的一部分。这样 **findMeetingTimes** 可查找适合于正在安排的活动类型的时间。有关详细信息，请参阅[请求正文](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_findmeetingtimes#request-body)部分。|
|添加项|Beta|支持以纯文本格式获取 **event** 正文，以作为默认 HTML 格式的替代选择。有关详细信息，请参阅 [get](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/event_get) 和 [list](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_list_events) 事件。|

### <a name="outlook-mail"></a>Outlook 邮件

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|更改|Beta|支持以纯文本格式获取 **message** 正文，以作为默认 HTML 格式的替代选择。有关详细信息，请参阅 [get](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/message_get) 和 [list](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_list_messages) 事件。|


### <a name="outlook-tasks"></a>Outlook 任务

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|Beta|向 [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/user) 添加新的 **outlook** 导航属性以访问  Outlook 任务。|
|添加项|Beta|新实体 [outlookuser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/outlookuser)、[outlookTaskGroup](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/outlooktaskgroup)、[outlookTaskFolder](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/outlooktaskfolder) 和 [outlookTask](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/outlooktask) 及其方法支持组织和访问 Outlook 任务。 | 
|添加项|Beta|Outlook 任务支持附件（[attachment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/attachment)、[fileAttachment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/fileattachment)、[itemAttachment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/itemattachment) 和 [referenceAttachment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/referenceattachment) 资源）。 |
|添加项|Beta|Outlook 任务支持[扩展的属性](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/extended-properties-overview)（[singleValueLegacyExtendedProperty](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/singlevaluelegacyextendedproperty) 和 [multiValueLegacyExtendedProperty](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/multivaluelegacyextendedproperty) 资源）。 |

### <a name="planner-apis"></a>规划器 API

|**更改类型**|**版本**|**说明**| 
|:-------------|:-----------|:--------------|
|添加项|v1.0|添加了[规划器 API](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/planner_overview)。<br />新资源：<br />[plannerPlan](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerPlan) <br />[plannerTask](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerTask) <br />[plannerPlanDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerPlanDetails) <br />[plannerTaskDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerTaskDetails) <br />[plannerBucket](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerBucket) <br />[plannerAssignedToTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerassignedtotaskboardtaskformat) <br />[plannerBucketTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerbuckettaskboardtaskformat) <br />[plannerProgressTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/plannerprogresstaskboardtaskformat) | 

### <a name="sharepoint-sites"></a>SharePoint 网站

|**更改类型**|**版本**|**说明**|
|:--------------|:----------|:--------------|
| 添加项      | v1.0      | 现在站点的资源在 v1.0 终结点中可用。<br/> 添加了 **site** 和 **siteCollection** 资源类型。
| 更改        | beta      | 已更改 **site** 资源的标识符格式。这是 beta API 中的重大更改。
| 已删除       | beta      | 从测试版 API 中删除了 **sharePoint** 实体。现在可在**网站**集中使用此功能。

### <a name="sharepoint-lists"></a>SharePoint 列表

|**更改类型**|**版本**|**说明**|
|:--------------|:----------|:--------------|
| 更改 | beta | 删除了 **sharepoint** 导航属性。现在可以通过 **sites** 导航属性直接访问站点。 <br/> 删除了 **fieldDefinition** 资源。它已被 **columnDefinition** 取代。 <br/> 从 **site** 删除了 **siteCollectionId** 和 **siteId** 属性。改为使用 **sharepointIds**。 <br/> 从 **listItem** 删除了 **listItemId** 属性。改为使用 **sharepointIds**。 <br/> 将 **listItem** 上的 **columnSet** 属性重命名为 **fields**。 <br/> 更改了 **site** 资源，以将 SharePoint 主机名用作其 ID。
| 添加项 | beta | 添加了 **booleanColumn**、**calculatedColumn**、**choiceColumn**、**dateTimeColumn**、**lookupColumn**、**numberColumn**、**personOrGroupColumn** 和 **textColumn** 资源类型。 <br/> 向 **site** 添加了 **displayName** 属性。 <br/> 向 **site** 添加了 **columns** 导航属性。 <br/> 向 **sharedDriveItem** 添加了 **list** 和 **listItem** 导航属性。 <br/> 向 **list** 和 **listItem** 以及 **site** 添加了 **sharepointIds** 属性。 <br/> 添加了 **columnDefinition** 资源类型。




## <a name="april-2017"></a>2017 年 4 月

### <a name="administrative-units-property-changes"></a>管理单元属性更改

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|更改|Beta| 管理单元 API 将在预览 (beta) 中得到更新。第一个更改集将于 2017 年 5 月 3 日应用。这些更改包括以下属性重命名：<br />scopedRoleMembership 实体的**标识**复杂类型的 - **roleMemberInfo** 复杂类型<br />用户实体的 **scopedRoleMemberOf** 的 - **scopedAdministratorOf** 导航属性<br />administrativeUnit 实体的 **scopedRoleMembers** 的 - **scopedAdministrators** 导航属性<br />directoryRole 实体的 **scopedMembers** 的 - **scopedAdministrators** 导航属性 |

### <a name="application-and-serviceprincipal-api-changes"></a>应用程序和 servicePrincipal API 更改

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|更改|Beta| [application](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/application) 和 [servicePrincipal](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/serviceprincipal) API 将在预览 (beta) 中得到更新。第一个更改集将于 2017 年 5 月 15 日应用。这些更改包括属性重命名和重构。在更改完成后，某些属性（如 appRoles 和 addIns）才可用。这些更改在发布到 v1.0 之前将先在预览版 (beta) 中发布。 |

### <a name="added-preview-support-for-cloud-solution-provider-developers"></a>添加了对云解决方案提供商开发人员的预览支持

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|Beta|添加新的预览功能以允许云解决方案提供商预先同意应用程序调用 Microsoft Graph，如新的[授权主题](https://graph.microsoft.io/en-us/docs/concepts/auth_cloudsolutionprovider)中所述。 |

### <a name="added-onpremises-properties-to-user-entity"></a>向用户实体添加了 onPremises 属性

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|Beta|向 [user](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/user) 实体添加了新的 onPremises 属性、onPremisesDomainName、OnPremisesSamAccountName 和 onPremisesUserPrincipalName。 |

### <a name="new-planner-apis-and-an-update-to-the-group-visibility-property"></a>新规划器 API 和对组可见性属性的更新

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|更改|Beta|向 [Group](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/group) 实体添加了 **HiddenMembership** 作为可见性属性的附加值 |
|添加项|Beta|添加了新的[规划器 API](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/planner_overview)。<br />新资源：<br />[plannerPlan](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerPlan) <br />[plannerTask](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerTask) <br />[plannerPlanDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerPlanDetails) <br />[plannerTaskDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerTaskDetails) <br />[plannerBucket](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerBucket) <br />[plannerAssignedToTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerassignedtotaskboardtaskformat) <br />[plannerBucketTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerbuckettaskboardtaskformat) <br />[plannerProgressTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerprogresstaskboardtaskformat) | 

### <a name="intune-apis"></a>Intune API
|**更改类型**|**版本**|**说明**|
|:---|:---|:---|
|添加项|Beta|添加的新实体：<br/>[androidForWorkCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcompliancepolicy)<br/>[deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate)<br/>[deviceInstallState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_deviceinstallstate)<br/>[deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscript)<br/>[deviceManagementScriptGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscriptgroupassignment)<br/>[deviceManagementScriptState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscriptstate)<br/>[eBookGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_ebookgroupassignment)<br/>[iosVppEBook](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_iosvppebook)<br/>[managedEBook](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_managedebook)<br/>[userInstallStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_userinstallstatesummary)<br/>[windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapp)<br/>[windowsManagementAppHealthState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapphealthstate)<br/>|
|添加项|Beta|添加的复杂类型：<br/>[dailySchedule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_dailyschedule)<br/>[hourlySchedule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_hourlyschedule)<br/>[iosBookmark](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosbookmark)<br/>[iosWebContentFilterAutoFilter](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterautofilter)<br/>[iosWebContentFilterBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterbase)<br/>[iosWebContentFilterSpecificWebsitesAccess](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterspecificwebsitesaccess)<br/>[runSchedule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_runschedule)<br/>[sharedAppleDeviceUser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedappledeviceuser)<br/>[windows10NetworkProxyServer](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10networkproxyserver)<br/>|
|添加项|Beta|在 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) 上添加了 [requestRemoteAssistance](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_requestremoteassistance) 操作 |
|添加项|Beta|在 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) 上添加了 [cleanWindowsDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_cleanwindowsdevice) 操作 |
|添加项|Beta|在 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) 上添加了 [logoutSharedAppleDeviceActiveUser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_logoutsharedappledeviceactiveuser) 操作 |
|添加项|Beta|在 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) 上添加了 [deleteUserFromSharedAppleDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_deleteuserfromsharedappledevice) 操作 |
|添加项|Beta|在 [deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscript) 上添加了 [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_devicemanagementscript_assign) 操作 |
|添加项|Beta|在 [appleVolumePurchaseProgramToken](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_applevolumepurchaseprogramtoken) 上添加了 [syncLicenses](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_onboarding_applevolumepurchaseprogramtoken_synclicenses) 操作 |
|添加项|Beta|在 [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) 集合上添加了 **getTopMobileApps** 函数 |
|添加项|Beta|在 [applePushNotificationCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_applepushnotificationcertificate) 上添加了 [downloadApplePushNotificationCertificateSigningRequest](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest) 函数 |
|添加项|Beta|在 [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) 上添加了 [getDeviceComplianceSettingStates](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_devicemanagement_getdevicecompliancesettingstates) 函数 |
|添加项|Beta|在 [reportRoot](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_reportroot) 上添加了 [deviceConfigurationUserActivity](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity) 函数 |
|添加项|Beta|在 [reportRoot](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_reportroot) 上添加了 [deviceConfigurationDeviceActivity](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity) 函数 |
|删除|Beta|删除了以下复杂类型：<br/>**enterpriseCloudResource**<br/>**windowsInformationProtectionAppRule**<br/>**windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate**<br/>**windowsInformationProtectionAppRuleDesktopTemplate**<br/>**windowsInformationProtectionAppRuleStoreAppTemplate**<br/>**windowsInformationProtectionAppRuleTemplate**<br/>**windowsInformationProtectionCorporateNetworkLocation**<br/>**windowsInformationProtectionProtectedLocation**<br/>**windowsInformationProtectionProtectedLocationEnterpriseCloudResources**<br/>**windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames**<br/>**windowsInformationProtectionProtectedLocationEnterpriseProxyServers**<br/>**windowsInformationProtectionProtectedLocationNeutralResources**<br/>|
|更改|Beta|向 [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) 实体添加了 **deviceSharingAllowed** 属性|
|更改|Beta|从 [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) 实体中删除了 **deviceSharingBlocked** 属性|
|更改|Beta|向 [defaultManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) 实体添加了 **minimumRequiredSdkVersion** 属性|
|更改|Beta|向 [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) 实体添加了 **windowsManagementAppEnabled** 属性|
|更改|Beta|向 [deviceComplianceActionItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceactionitem) 实体添加了 **notificationTemplateId** 属性|
|更改|Beta|向 [deviceConfigurationGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationgroupassignment) 实体添加了 **excludeGroup** 属性|
|更改|Beta|更改了 [iosCustomConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscustomconfiguration) 实体上的以下属性：<br/>将 **payloadFileName** 从必需更改为可选<br/>|
|更改|Beta|向 [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration) 实体添加了 **contentFilterSettings** 属性|
|更改|Beta|向 [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) 实体添加了 **cellularBlockPersonalHotspot** 和 **passcodeBlockFingerprintModification** 属性|
|更改|Beta|向 [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) 实体添加了 **minimumRequiredSdkVersion** 属性|
|更改|Beta|更改了 [macOSCustomConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscustomconfiguration) 实体上的以下属性：<br/>将 **payloadFileName** 从必需更改为可选<br/>|
|更改|Beta|向 [managedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedappprotection) 实体添加了 **disableAppPinIfDevicePinIsSet**、**minimumRequiredOsVersion**、**minimumWarningOsVersion**、**minimumRequiredAppVersion** 和 **minimumWarningAppVersion** 属性|
|更改|Beta|向 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) 实体添加了 **remoteAssistanceSessionUrl**、**isEncrypted**、**model** 和 **manufacturer** 属性|
|更改|Beta|更改了 [getMobileAppCount](https://developer.microsoft.com/en-us/graph/docs/docs/api-reference/beta/api/intune_apps_mobileapp_getmobileappcount) 实体上的以下属性：<br/>将 **bindingParameter** 从 **mobileApp** 更改为 *mobileApp* 的**集合**<br/>将 **status** 从 GUID 更改为字符串<br/>|
|更改|Beta|向 [mobileAppGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappgroupassignment) 实体添加了 **vpnConfigurationId** 属性|
|更改|Beta|从 [notificationMessageTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_notificationmessagetemplate) 实体中删除了 **fromEmailAddress** 属性|
|更改|Beta|向 [officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp) 实体添加了 **excludedApps** 属性|
|更改|Beta|从 [officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp) 实体中删除了 **excludedOfficeApps** 属性|
|更改|Beta|向 [sharedPCConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcconfiguration) 实体添加了 **enabled** 属性|
|更改|Beta|向 [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) 实体添加了 **networkProxyApplySettingsDeviceWide**、**networkProxyDisableAutoDetect**、**networkProxyAutomaticConfigurationUrl**、**networkProxyServer**、**bluetoothDeviceName**、**wiFiScanInterval**、**wirelessDisplayBlockProjectionToThisDevice**、**wirelessDisplayBlockUserInputFromReceiver**、**wirelessDisplayRequirePinForPairing**、**experienceBlockDeviceDiscovery**、**experienceBlockErrorDialogWhenNoSIM**、**experienceBlockTaskSwitcher**、**startMenuPinnedFolderDocuments**、**startMenuPinnedFolderDownloads**、**startMenuPinnedFolderFileExplorer**、**startMenuPinnedFolderHomeGroup**、**startMenuPinnedFolderMusic**、**startMenuPinnedFolderNetwork**、**startMenuPinnedFolderPersonalFolder**、**startMenuPinnedFolderPictures**、**startMenuPinnedFolderSettings**、**startMenuPinnedFolderVideos**、**startMenuAppListVisibility**、**startMenuHideFrequentlyUsedApps**、**startMenuHideRecentJumpLists**、**startMenuHideRecentlyAddedApps**、**startMenuHideRestartOptions**、**startMenuHideUserTile**、**startMenuHidePowerButton**、**startMenuLayoutEdgeAssetsXml**、**personalizationDesktopImageUrl** 和 **personalizationLockScreenImageUrl** 属性|
|更改|Beta|更改了 [windowsMobileMSI](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi) 实体上以下属性的类型：<br/>将 **productCode** 从 Guid 更改为字符串<br/>|
|更改|Beta|更改了 [windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx) 实体上的以下属性：<br/>将 **phoneProductIdentifier** 从必需更改为可选<br/>将 **phonePublisherId** 从必需更改为可选<br/>|
|更改|Beta|更改了 [windowsPhone81AppXBundle](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appxbundle) 实体上的以下属性：<br/>将 **appXPackageInformationList** 从必需更改为可选<br/>|
|更改|Beta|向 [windowsStoreForBusinessApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessapp) 实体添加了 **productKey** 和 **licenseType** 属性|
|更改|Beta|向 [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration) 实体添加了 **previewBuildSetting** 属性|
|更改|Beta|向 [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) 实体添加了 **windowsManagementApp** 和 **managedEBooks** 导航属性|
|更改|Beta|向 [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) 实体添加了 **deviceManagementScripts**、**managedDeviceOverview** 和 **cloudPkiSubscriptions** 导航属性|
|更改|Beta|向 [deviceEnrollmentPlatformRestrictions](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_deviceenrollmentplatformrestrictions) 复杂类型添加了 **osMinimumVersion** 和 **osMaximumVersion** 属性|
|更改|Beta|向 [hardwareInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_hardwareinformation) 复杂类型添加了 **isSharedDevice** 和 **sharedDeviceCachedUsers** 属性|
|更改|Beta|更改了 [omaSettingBase64](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_omasettingbase64) 复杂类型上的以下属性：<br/>将 **fileName** 从必需更改为可选<br/>|
|更改|Beta|更改了 [omaSettingStringXml](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_omasettingstringxml) 复杂类型上的以下属性：<br/>将 **fileName** 从必需更改为可选<br/>|

## <a name="march-2017"></a>2017 年 3 月

### <a name="intune-apis"></a>Intune API

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|Beta|添加的新实体：<br/>[androidForWorkApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidforworkapp)<br/>[androidForWorkAppConfigurationSchema](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschema)<br/>[androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings)<br/>[androidForWorkVpnConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkvpnconfiguration)<br/>[applePushNotificationCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_applepushnotificationcertificate)<br/>[complianceSettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_compliancesettingstatesummary)<br/>[deviceCompliancePolicyDeviceStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary)<br/>[deviceCompliancePolicyState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicystate)<br/>[deviceConfigurationDeviceStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatesummary)<br/>[deviceConfigurationState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationstate)<br/>[enterpriseCodeSigningCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_enterprisecodesigningcertificate)<br/>[iosEduDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosedudeviceconfiguration)<br/>[managedDeviceCertificateState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevicecertificatestate)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicesummary)<br/>[managedDeviceMobileAppConfigurationUserSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationusersummary)<br/>[mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_mdmwindowsinformationprotectionpolicy)<br/>[mobileAppInstallSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallsummary)<br/>[mobileAppProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappprovisioningconfiggroupassignment)<br/>[mobileThreatDefenseConnector](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_mobilethreatdefenseconnector)<br/>[officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp)<br/>[settingStateDeviceSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_settingstatedevicesummary)<br/>[softwareUpdateStatusSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_softwareupdatestatussummary)<br/>[symantecCodeSigningCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_symanteccodesigningcertificate)<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration)<br/>[windowsInformationProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection)<br/>[windowsInformationProtectionAppLockerFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapplockerfile)<br/>[windowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy)<br/>[windowsMobileMSI](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi)<br/>|
|添加项|Beta|添加的复杂类型：<br/>[androidForWorkAppConfigurationExample](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexample)<br/>[androidForWorkAppConfigurationExampleJson](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexamplejson)<br/>[androidForWorkAppConfigurationSchemaItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschemaitem)<br/>[deviceCompliancePolicySettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate)<br/>[deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate)<br/>[deviceExchangeAccessStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceexchangeaccessstatesummary)<br/>[edgeSearchEngine](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchengine)<br/>[edgeSearchEngineBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchenginebase)<br/>[edgeSearchEngineCustom](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchenginecustom)<br/>[excludedApps](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_excludedapps)<br/>[iosEduCertificateSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducertificatesettings)<br/>[ipRange](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iprange)<br/>[windowsInformationProtectionApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapp)<br/>[windowsInformationProtectionCloudResource](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioncloudresource)<br/>[windowsInformationProtectionCloudResourceCollection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioncloudresourcecollection)<br/>[windowsInformationProtectionDesktopApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondesktopapp)<br/>[windowsInformationProtectionIPRangeCollection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioniprangecollection)<br/>[windowsInformationProtectionResourceCollection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionresourcecollection)<br/>[windowsInformationProtectionStoreApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionstoreapp)<br/>|
|添加项|Beta|在 [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) 上添加了 [requestSignupUrl](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_requestsignupurl) 操作 |
|添加项|Beta|在 [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) 上添加了 [completeSignup](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_completesignup) 操作 |
|添加项|Beta|在 [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) 上添加了 [syncApps](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_syncapps) 操作 |
|添加项|Beta|在 [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) 上添加了 [unbind](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_unbind) 操作 |
|添加项|Beta|在 [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) 上添加了 [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign) 操作 |
|添加项|Beta|在 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) 上添加了 [recoverPasscode](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_recoverpasscode) 操作 |
|添加项|Beta|在 [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_organization) 上添加了 [removeApplePushNotificationCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_onboarding_organization_removeapplepushnotificationcertificate) 操作 |
|添加项|Beta|在 [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) 上添加了 [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_iosmanagedappprotection_updatemobileappidentifierdeployments) 操作 |
|添加项|Beta|在 [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) 上添加了 [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_androidmanagedappprotection_updatemobileappidentifierdeployments) 操作 |
|添加项|Beta|在 [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) 上添加了 [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_updatemobileappidentifierdeployments) 操作 |
|添加项|Beta|在 [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) 上添加了 [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_iosmanagedappprotection_updatetargetedsecuritygroups) 操作 |
|添加项|Beta|在 [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) 上添加了 [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_androidmanagedappprotection_updatetargetedsecuritygroups) 操作 |
|添加项|Beta|在 [windowsInformationProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) 上添加了 [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_windowsinformationprotection_updatetargetedsecuritygroups) 操作 |
|添加项|Beta|在 [windowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy) 上添加了 [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_windowsinformationprotection_updatetargetedsecuritygroups) 操作 |
|添加项|Beta|在 [mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_mdmwindowsinformationprotectionpolicy) 上添加了 [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_mdmwindowsinformationprotectionpolicy_updatetargetedsecuritygroups) 操作 |
|添加项|Beta|在 [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_user) 上添加了 [wipeManagedAppRegistrationByDeviceTag](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_user_wipemanagedappregistrationbydevicetag) 操作 |
|添加项|Beta|在 [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) 上添加了 [getTopMobileApps](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_apps_mobileapp_gettopmobileapps) 函数 |
|添加项|Beta|在 [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) 上添加了 [verifyWindowsEnrollmentAutoDiscovery](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_corpenrollment_devicemanagement_verifywindowsenrollmentautodiscovery) 函数 |
|删除|Beta|删除了以下实体：<br/>**appProvisioningConfigGroupAssignment**<br/>**defaultManagedAppConfiguration**<br/>**enterpriseCertificate**<br/>**managedDeviceMobileAppProvisioningConfigurationDeviceStatus**<br/>**symantecCertificate**<br/>**windows10WindowsInformationProtectionConfiguration**<br/>|
|删除|Beta|删除了以下复杂类型：<br/>**mobileAppInstallSummary**<br/>**windowsArchitecture**<br/>**windowsDeviceType**<br/>|
|更改|Beta|向 [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) 实体添加了 **webBrowserBlockPopups** 属性|
|更改|Beta|从 [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) 实体中删除了 **webBrowserAllowPopups** 属性|
|更改|Beta|向 [androidStoreApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidstoreapp) 实体添加了 **appIdentifier** 属性|
|更改|Beta|从 [appReportingOverviewStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/appReportingOverviewStatus) 实体中删除了 **applicationCount**、**failedApplicationCount** 和 **appInstallFailures** 属性|
|更改|Beta|向 [depEnrollmentProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_corpenrollment_depenrollmentprofile) 实体添加了 **sharedIPadMaximumUserCount** 和 **enableSharedIPad** 属性|
|更改|Beta|向 [depOnboardingSetting](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_deponboardingsetting) 实体添加了 **shareTokenWithSchoolDataSyncService** 和 **lastSyncErrorCode** 属性|
|更改|Beta|向 [deviceComplianceDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview) 实体添加了 **pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime** 和 **configurationVersion** 属性|
|更改|Beta|从 [deviceComplianceDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview) 实体中删除了 **numberOfPendingDevices**、**numberOfSucceededDevices**、**numberOfErrorDevices**、**numberOfFailedDevices**、**lastUpdateTime** 和 **policyRevision** 属性|
|更改|Beta|向 [deviceComplianceUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview) 实体添加了 **pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime** 和 **configurationVersion** 属性|
|更改|Beta|从 [deviceComplianceUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview) 实体中删除了 **numberOfPendingUsers**、**numberOfSucceededUsers**、**numberOfErrorUsers**、**numberOfFailedUsers**、**lastUpdateTime** 和 **policyRevision** 属性|
|更改|Beta|向 [deviceConfigurationDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview) 实体添加了 **pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime** 和 **configurationVersion** 属性|
|更改|Beta|从 [deviceConfigurationDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview) 实体中删除了 **numberOfPendingDevices**、**numberOfSucceededDevices**、**numberOfErrorDevices**、**numberOfFailedDevices**、**lastUpdateTime** 和 **policyRevision** 属性|
|更改|Beta|向 [deviceConfigurationUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview) 实体添加了 **pendingCount**、**successCount**、**errorCount**、**failedCount**、**lastUpdateDateTime** 和 **configurationVersion** 属性|
|更改|Beta|从 [deviceConfigurationUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview) 实体中删除了 **numberOfPendingUsers**、**numberOfSucceededUsers**、**numberOfErrorUsers**、**numberOfFailedUsers**、**lastUpdateTime** 和 **policyRevision** 属性|
|更改|Beta|向 [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) 实体添加了 **subscriptionState** 属性|
|更改|Beta|向 [iosCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscompliancepolicy) 实体添加了 **managedEmailProfileRequired** 属性|
|更改|Beta|向 [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) 实体添加了 **appsSingleAppModeList** 属性|
|更改|Beta|从 [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) 实体中删除了 **appsSingleAppModeBundleIds** 属性|
|更改|Beta|向 [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) 实体添加了 **expirationDateTime** 属性|
|更改|Beta|从 [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) 实体中删除了 **expiration** 属性|
|更改|Beta|向 [macOSCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscompliancepolicy) 实体添加了 **passwordMinimumCharacterSetCount**、**osMinimumVersion**、**osMaximumVersion**、**deviceThreatProtectionEnabled**、**deviceThreatProtectionRequiredSecurityLevel** 和 **storageRequireEncryption** 属性|
|更改|Beta|从 [managedAndroidLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp) 实体中删除了 **manifest** 属性|
|更改|Beta|向 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) 实体添加了 **isSupervised**、**exchangeLastSuccessfulSyncDateTime**、**exchangeAccessState** 和 **exchangeAccessStateReason** 属性|
|更改|Beta|向 [managedDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddeviceoverview) 实体添加了 **deviceExchangeAccessStateSummary** 属性|
|更改|Beta|从 [managedIOSLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp) 实体中删除了 **manifest** 属性|
|更改|Beta|从 [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) 实体中删除了 **installSummary** 属性|
|更改|Beta|向 [mobileAppContentFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile) 实体添加了 **uploadState** 属性|
|更改|Beta|更改了 [mobileAppContentFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile) 实体上的以下属性：<br/>将 **azureStorageUriExpirationDateTime** 从必需更改为可选<br/>|
|更改|Beta|向 [remoteActionAudit](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_remoteactionaudit) 实体添加了 **initiatedByUserPrincipalName**、**deviceOwnerUserPrincipalName**、**deviceIMEI** 和 **actionState** 属性|
|更改|Beta|向 [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) 实体添加了 **oneDriveDisableFileSync**、**safeSearchFilter**, **edgeSearchEngine**、**settingsBlockSettingsApp**、**settingsBlockSystemPage**、**settingsBlockDevicesPage**、**settingsBlockNetworkInternetPage**、**settingsBlockPersonalizationPage**、**settingsBlockAccountsPage**、**settingsBlockTimeLanguagePage**、**settingsBlockEaseOfAccessPage**、**settingsBlockPrivacyPage**、**settingsBlockUpdateSecurityPage**、**experienceBlockWindowsSpotlight**、**experienceBlockWindowsTips**、**experienceBlockConsumerSpecificFeatures**、**startMenuLayoutXml**、**startMenuMode**、**logonBlockFastUserSwitching** 和 **startBlockUnpinningAppsFromTaskbar** 属性|
|更改|Beta|向 [windows10SecureAssessmentConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration) 实体添加了 **allowPrinting**、**allowScreenCapture** 和 **allowTextSuggestion** 属性|
|更改|Beta|从 [windows10SecureAssessmentConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration) 实体中删除了 **blockPrinting**、**blockScreenCapture** 和 **blockTextSuggestion** 属性|
|更改|Beta|向 [windowsAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsappx) 实体添加了 **identityName** 属性|
|更改|Beta|更改了 [windowsAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsappx) 实体上以下属性的类型：<br/>将 **applicableArchitectures** 从 [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture) 更改为字符串<br/>|
|更改|Beta|向 [windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx) 实体添加了 **identityName** 属性|
|更改|Beta|更改了 [windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx) 实体上以下属性的类型：<br/>将 **applicableArchitectures** 从 [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture) 更改为字符串<br/>|
|更改|Beta|向 [windowsUniversalAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx) 实体添加了 **identityName**、**identityPublisherHash** 和 **identityResourceIdentifier** 属性|
|更改|Beta|更改了 [windowsUniversalAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx) 实体上以下属性的类型：<br/>将 **applicableArchitectures** 从 [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture) 更改为字符串<br/>将 **applicableDeviceTypes** 从 [windowsDeviceType](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsDeviceType) 更改为字符串<br/>|
|更改|Beta|向 [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration) 实体添加了 **restartMode** 属性|
|更改|Beta|向 [androidForWorkScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile) 实体添加了 **managedDeviceCertificateStates** 导航属性|
|更改|Beta|向 [androidScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidscepcertificateprofile) 实体添加了 **managedDeviceCertificateStates** 导航属性|
|更改|Beta|向 [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) 实体添加了 **enterpriseCodeSigningCertificates**、**symantecCodeSigningCertificate**、**sideLoadingKeys**、**managedAppPolicies**、**iosManagedAppProtections**、**androidManagedAppProtections**、**defaultManagedAppProtections**、**targetedManagedAppConfigurations**、**mdmWindowsInformationProtectionPolicies**、**windowsInformationProtectionPolicies**、**managedAppRegistrations** 和 **managedAppStatuses** 导航属性|
|更改|Beta|从 [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) 实体中删除了 **appReportingOverview**、**enterpriseCerts** 和 **symantecCert** 导航属性|
|更改|Beta|向 [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) 实体添加了 **deviceSettingStateSummaries** 导航属性|
|更改|Beta|向 [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) 实体添加了 **deviceSettingStateSummaries** 导航属性|
|更改|Beta|向 [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) 实体添加了 **termsAndConditions**、**androidForWorkSettings**、**androidForWorkAppConfigurationSchemas**、**applePushNotificationCertificate**、**softwareUpdateStatusSummary**、**deviceCompliancePolicyDeviceStateSummary**、**complianceSettingStateSummaries**、**deviceConfigurationDeviceStateSummaries** 和 **mobileThreatDefenseConnectors** 导航属性|
|更改|Beta|从 [iosEducationDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration) 实体删除了 **teacherRootCertificates**、**teacherIdentityCertificate**、**studentRootCertificates** 和 **studentIdentityCertificate** 导航属性|
|更改|Beta|更改了 [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) 实体上以下属性的类型：<br/>将 **deviceStatuses** 从 [managedDeviceMobileAppProvisioningConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/managedDeviceMobileAppProvisioningConfigurationDeviceStatus) 集合更改为 [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus) 集合<br/>将 **groupAssignments** 从 [appProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/appProvisioningConfigGroupAssignment) 集合更改为 [mobileAppProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappprovisioningconfiggroupassignment) 集合<br/>|
|更改|Beta|向 [iosScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosscepcertificateprofile) 实体添加了 **managedDeviceCertificateStates** 导航属性|
|更改|Beta|向 [macOSScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosscepcertificateprofile) 实体添加了 **managedDeviceCertificateStates** 导航属性|
|更改|Beta|向 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) 实体添加了 **deviceConfigurationStates** 和 **deviceCompliancePolicyStates** 导航属性|
|更改|Beta|向 [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration) 实体添加了 **deviceStatusSummary** 和 **userStatusSummary** 导航属性|
|更改|Beta|向 [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) 实体添加了 **installSummary** 导航属性|
|更改|Beta|从 [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_organization) 实体中删除了 **sideLoadingKeys** 导航属性|
|更改|Beta|向 [windows81SCEPCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81scepcertificateprofile) 实体添加了 **managedDeviceCertificateStates** 导航属性|
|更改|Beta|向 [windowsPhone81SCEPCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81scepcertificateprofile) 实体添加了 **managedDeviceCertificateStates** 导航属性|
|更改|Beta|从 [appInstallationFailure](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure) 复杂类型中删除了 **applicationId**、**appName**、**platformId**、**userFailures** 和 **deviceFailures** 属性|
|更改|Beta|向 [iosHomeScreenFolderPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolderpage) 复杂类型添加了 **displayName** 属性|
|更改|Beta|向 [iosHomeScreenPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenpage) 复杂类型添加了 **displayName** 属性|
|更改|Beta|向 [windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate) 复杂类型添加了 **subjectName**、**description**、**expirationDateTime** 和 **certificate** 属性|
|更改|Beta|从 [windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate) 复杂类型中删除了 **dataRecoveryCertificate** 和 **certificateFileName** 属性|
|更改|Beta|向 [windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation) 复杂类型添加了 **displayName** 属性|
|更改|Beta|更改了 [windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation) 复杂类型上以下属性的类型：<br/>将 **applicableArchitecture** 从 [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture) 更改为字符串<br/>|
|更改|Beta|更改了 [windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation) 复杂类型上的以下属性：<br/>将 **applicableArchitecture** 从可选更改为必需<br/>|

### <a name="add-contracts-to-microsoft-graph"></a>将协定添加到 Microsoft Graph

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|Beta|新资源：</br>[contract](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/contract) |

### <a name="add-domain-operations-to-microsoft-graph"></a>将域操作添加到 Microsoft Graph

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|Beta|在[域](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domain)上添加了函数。<br/>新实体：</br>[domain](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domain)<br/>[domainDnsRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domaindnsrecord)<br/>[domainDnsCnameRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsCnameRecord)<br/>[domainDnsMxRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsMxRecord)<br/>[domainDnsSrvRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsSrvRecord)<br/>[domainDnsTxtRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsTxtRecord)<br/>[domainDnsUnavailableRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsUnavailableRecord)<br/>新操作：</br>[forceDelete](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/domain_forcedelete)</br>[verify](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/domain_verify) |

### <a name="add-custom-data-to-microsoft-graph-using-schema-extensions"></a>使用架构扩展将自定义数据添加到 Microsoft Graph

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|Beta|使用[架构扩展](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_overview#schema-extensions-preview)通过应用程序数据扩展 Microsoft Graph。该操作在以下资源上受支持：<br/>管理单元<br/>日历事件<br/>设备<br/>组<br/>消息<br/>组织<br/>个人联系人<br/>帖子<br/>用户<br/>请参阅以下示例：<br/>[使用架构扩展向组添加自定义数据（预览）](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_schema_groups)|
|添加项|Beta|提供另一种不需要验证的 .com 虚域就能创建架构扩展定义的方法。有关详细信息，请参阅[架构扩展](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_overview#schema-extensions-preview)。|

### <a name="add-custom-data-to-microsoft-graph-using-open-extensions"></a>使用开放扩展将自定义数据添加到 Microsoft Graph。

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|更改| v1.0 和 beta | 将前述“Office 365 数据扩展”重命名为“开放扩展”。 |
|添加项|Beta|已添加支持[开放扩展](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_overview#open-extensions)的资源： <br/>管理单元<br/>设备<br/>组<br/>组织<br/>用户<br/>请参阅以下示例：<br/>[使用开放扩展向用户添加自定义数据（预览）](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_open_users)|

### <a name="directory-apis"></a>目录 API

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|Beta|已添加对[还原并永久删除组](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/directory)的支持。<br/>新实体：带有 deleteditems 导航属性的目录。 |
|添加项|Beta|新实体：</br>[终结点](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/endpoint) |
|更改  |Beta|针对[组](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/group)的新 [endpoints](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/group_list_endpoints) 导航属性 |
|添加项|Beta|新实体：</br>[licenseDetails](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/licensedetails) |
|更改  |Beta|针对[用户](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/user)的新 [licensedetails](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/user_list_licensedetails) 导航属性 |

### <a name="reports-apis"></a>报表 API

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|Beta|Office 365 报表引入的新预览 API。可用于获取用户在业务中如何使用 Office 365 服务的使用情况报告。例如，你可以确定大量使用服务并达到配额的用户，或者可能完全不需要 Office 365 许可证的用户。有关详细信息，请参阅[报表](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/report)。|

### <a name="directory-apis"></a>目录 API

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|Beta|新实体：</br>[contract](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/contract) |

## <a name="february-2017"></a>2017 年 2 月

### <a name="intune-apis"></a>Intune API

|更改类型|版本|说明|
|:---|:---|:---|
|添加项|Beta|增加了新实体：<br/>[androidForWorkCertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcertificateprofilebase)<br/>[androidForWorkEasEmailProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkeasemailprofilebase)<br/>[androidForWorkEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkenterprisewificonfiguration)<br/>[androidForWorkGmailEasConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgmaileasconfiguration)<br/>[androidForWorkNineWorkEasConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworknineworkeasconfiguration)<br/>[androidForWorkPkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkpkcscertificateprofile)<br/>[androidForWorkScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile)<br/>[androidForWorkTrustedRootCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworktrustedrootcertificate)<br/>[androidForWorkWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkwificonfiguration)<br/>[appleDeviceFeaturesConfigurationBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_appledevicefeaturesconfigurationbase)<br/>[appProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appprovisioningconfiggroupassignment)<br/>[deviceComplianceUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview)<br/>[deviceConfigurationUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview)<br/>[enterpriseCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_enterprisecertificate)<br/>[iosEducationDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)<br/>[macOSDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosdevicefeaturesconfiguration)<br/>[managedAndroidLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp)<br/>[managedDeviceMobileAppProvisioningConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappprovisioningconfigurationdevicestatus)<br/>[managedIOSLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp)<br/>[managedMobileLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedmobilelobapp)<br/>[symantecCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_symanteccertificate)<br/>[windowsAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsappx)<br/>[windowsCertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase)<br/>[windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx)<br/>[windowsPhone81AppXBundle](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appxbundle)<br/>[windowsPhoneXAP](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphonexap)<br/>[windowsUniversalAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx)<br/>|
|添加项|Beta|新增了复杂类型：<br/>[airPrintDestination](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_airprintdestination)<br/>[windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsarchitecture)<br/>[windowsDeviceType](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsdevicetype)<br/>[windowsMinimumOperatingSystem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsminimumoperatingsystem)<br/>[windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation)<br/>|
|添加项|Beta|在 [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) 实体上添加了 [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign) 操作|
|添加项|Beta|在 [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) 实体上添加了 [scheduleActionsForRules](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_devicecompliancepolicy_scheduleactionsforrules) 操作|
|添加项|Beta|在 [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) 实体上添加了 [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_updatetargetedsecuritygroups) 操作|
|添加项|Beta|在 [resourceOperation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_rbac_resourceoperation) 实体上添加了 [getScopesForUser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_rbac_resourceoperation_getscopesforintune_devices_user) 函数|
|更改|Beta|从 [androidLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidlobapp) 实体中删除了 **manifest** 属性|
|更改|Beta|向 [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration) 实体添加了 **assetTagTemplate****lockScreenFootnote****homeScreenDockIcons** 和 **homeScreenPages** 属性|
|更改|Beta|从 [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration) 实体删除了 **deviceSharingAssetTagInformation**、**deviceSharingLockScreenFootnote**、**homeScreenLayoutDockIcons** 和 **homeScreenLayoutPages** 属性|
|更改|Beta|向 [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) 实体添加了 **appsSingleAppModeBundleIds** 属性|
|更改|Beta|从 [iosLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobapp) 实体删除了 **manifest** 属性|
|更改|Beta|向 [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) 实体添加了 **createdDateTime**、**description**、**lastModifiedDateTime**、**displayName** 和 **version** 属性|
|更改|Beta|向 [managedAppPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy) 实体添加了 **createdDateTime** 和 **lastModifiedDateTime** 属性|
|更改|Beta|从 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) 实体删除了 **deviceRegistrationState** 属性|
|更改|Beta|向 [mobileAppContentFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile) 实体添加了 **manifest** 属性|
|更改|Beta|向 [mobileAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus) 实体添加了 **osDescription** 和 **userName** 属性|
|更改|Beta|从 [mobileAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus) 实体删除了 **deviceType** 属性|
|更改|Beta|更改了 [mobileAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus) 实体以下属性的类型：<br/>将 **mobileAppInstallStatusValue** 从 Int32 更改为字符串|
|更改|Beta|向 [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) 实体添加了 **targetedSecurityGroupIds** 和 **targetedSecurityGroupsCount** 属性|
|更改|Beta|从 [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) 实体删除了 **numberOfTargetedSecurityGroups** 属性|
|更改|Beta|向 [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devices_user) 实体添加了 **id** 属性|
|更改|Beta|从 [windows10CertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10certificateprofilebase) 实体删除了 **renewalThresholdPercentage**、**keyStorageProvider**、**subjectNameFormat**、**subjectAlternativeNameType**、**certificateValidityPeriodValue** 和 **certificateValidityPeriodScale** 属性|
|更改|Beta|从 [windows81CertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81certificateprofilebase) 实体删除了 **renewalThresholdPercentage**、**keyStorageProvider**、**subjectNameFormat**、**subjectAlternativeNameType**、**certificateValidityPeriodValue** 和 **certificateValidityPeriodScale** 属性|
|更改|Beta|从 [windowsPhone81GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81generalconfiguration) 实体删除了 **applyToWindows10Mobile** 属性|
|更改|Beta|向 [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) 实体添加了 **enterpriseCerts**、**iosLobAppProvisioningConfigurations** 和 **symantecCert** 导航属性|
|更改|Beta|向 [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) 实体添加了 **userStatusOverview** 导航属性|
|更改|Beta|向 [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) 实体添加了 **userStatusOverview** 导航属性|
|更改|Beta|向 [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) 实体添加了 **groupAssignments**、**deviceStatuses** 和 **userStatuses** 导航属性|
|更改|Beta|更改了 [windows10VpnConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10vpnconfiguration) 实体上以下属性的类型：<br/>将 **identityCertificate** 从 [windows10CertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10certificateprofilebase) 更改为 [windowsCertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase)|
|更改|Beta|向 [deviceManagementSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) 复杂类型添加了 **deviceComplianceCheckinThresholdDays** 和 **isScheduledActionEnabled** 属性|
|更改|Beta|从 [deviceManagementSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) 复杂类型删除了 **windowsCommercialId** 和 **windowsCommercialIdLastModifiedTime** 属性|
|更改|Beta|向 [iosNotificationSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings) 复杂类型添加了 **bundleID**、**appName**、**publisher**、**enabled** 和 **showOnLockScreen** 属性|
|更改|Beta|从 [iosNotificationSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings) 复杂类型删除了 **bundleIdentifier**、**notificationsEnabled** 和 **showInLockScreen** 属性|



## <a name="january-2017"></a>2017 年 1 月

### <a name="outlook-calendar"></a>Outlook 日历

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|v1.0|
  [用户](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user)资源的新操作 [findMeetingTimes](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_findmeetingtimes)。|
|添加项|v1.0|新复杂类型 [attendeeBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/attendeebase)，由 attendee 类型的类型属性组成。|
|添加项|v1.0|新复杂类型：<br/>[attendeeAvailability](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/attendeeavailability)<br/>[locationConstraint](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/locationconstraint) <br/>[locationConstraintItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/locationconstraintitem)<br/>[meetingTimeSuggestion](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/meetingtimesuggestion)<br/>[meetingTimeSuggestionsResult](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/meetingtimesuggestionsresult)<br/>[timeConstraint](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/timeconstraint)<br/>[timeSlot](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/timeslot)|
|更改|v1.0|
  [attendee](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/attendee) 复杂类型现派生自 attendeeBase，而 attendeeBase 派生自 [recipient](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/recipient)。包括继承的属性在内，它同以前一样，由 **status**、**type** 和 **emailAddress** 属性组成。|
|添加项|Beta|添加到[日历](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/calendar)资源的 hexColor。|

### <a name="intune-apis"></a>Intune API

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|Beta|添加的新实体： <br/>[appReportingOverviewStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appreportingoverviewstatus)<br/>[deviceComplianceDeviceOverview](https://developer.microsoft.com/en-us/graph/docs//api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview)<br/>[deviceConfigurationDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview)<br/>[deviceManagementExchangeOnpremisesPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_devicemanagementexchangeonpremisespolicy)<br/>[iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)<br/>[iosEducationDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)<br/>[iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)<br/>[onpremisesConditionalAccessSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_onpremisesconditionalaccesssettings)<br/>[sharedPCConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcconfiguration)<br/>[windows10EnterpriseModernAppManagementConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration)<br/>[windows10SecureAssessmentConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration)<br/>[windows10WindowsInformationProtectionConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10windowsinformationprotectionconfiguration)|
|添加|Beta|新增了复杂类型： <br/> [appInstallationFailure](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure)<br/>[enterpriseCloudResource](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_enterprisecloudresource)<br/>[iosHomeScreenApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenapp)<br/>[iosHomeScreenFolder](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolder)<br/>[iosHomeScreenFolderPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolderpage)<br/>[iosHomeScreenItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenitem)<br/>[iosHomeScreenPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenpage)<br/>[iosNotificationSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings)<br/>[iPv6Range](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ipv6range)<br/>[sharedPCAccountManagerPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcaccountmanagerpolicy)<br/>[windowsInformationProtectionAppRule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionapprule)<br/>[windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruleapplockerpolicyfiletemplate)<br/>[windowsInformationProtectionAppRuleDesktopTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruledesktoptemplate)<br/>[windowsInformationProtectionAppRuleStoreAppTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionapprulestoreapptemplate)<br/>[windowsInformationProtectionAppRuleTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruletemplate)<br/>[windowsInformationProtectionCorporateNetworkLocation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectioncorporatenetworklocation)<br/>[windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectiondatarecoverycertificate)<br/>[windowsInformationProtectionProtectedLocation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocation)<br/>[windowsInformationProtectionProtectedLocationEnterpriseCloudResources](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterprisecloudresources)<br/>[windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseinternalproxyservers)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseipv4ranges)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseipv6ranges)<br/>[windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterprisenetworkdomainnames)<br/>[windowsInformationProtectionProtectedLocationEnterpriseProxyServers](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseproxyservers)<br/>[windowsInformationProtectionProtectedLocationNeutralResources](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationneutralresources)
|删除|beta|删除了以下复杂类型，并替换为 microsoft.graph.Json：<br/>managedAppDeploymentSummary <br/>managedAppSummary<br /> |
|更改|Beta|已将以下实体的属性类型从 appConfigComplianceStatus 替换为 complianceStatus： <br/>[managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus)<br/>[managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationuserstatus)|
|更改|beta|对于资源 [managedAppStatusRaw](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedappstatusraw)，已将属性内容的类型从 managedAppSummary 更改为 Json。|
|更改|beta|从 [managedAppRegistration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedappregistration) 集合中删除了 getUsersWithFlaggedAppRegistration 函数。|
|更改|beta|已将 [iosVppApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_iosvppapp) 实体的 **vppToken** 导航属性更改为不再是包含的集合。|
|更改|beta|向 [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) 和 [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) 实体添加了 **deviceStatusOverview** 属性。|
|更改|beta|向 [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) 单一实例添加了 **appReportingOverview** 属性。|
|更改|beta|向 [deviceConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus)、[deviceComplianceDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus) 和 [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus) 实体添加了 **deviceDisplayName** 和 **userPrincipalName** 属性。|
|更改|beta|向 [deviceComplianceScheduledActionForRule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancescheduledactionforrule) 实体添加了 **ruleName** 属性。|
|更改|beta|向 [deviceConfigurationUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuserstatus)、[deviceComplianceUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuserstatus) 和 [managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationuserstatus) 实体添加了 **devicesCount**、**userDisplayName** 和 **userPrincipalName** 属性。|
|更改|beta|向 [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagement) 单一实例添加了 [notificationMessageTemplates](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_notification_notificationmessagetemplate) 集合。|
|更改|beta|向 [localizedNotificationMessage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_localizednotificationmessage) 实体添加了 **isDefault**、**lastModifiedDateTime**、**locale**、**messageTemplate** 和 **subject** 属性。|
|更改|beta|向 [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_manageddevice) 实体添加了 **azureActiveDirectoryDeviceId**、**deviceCategory**、**deviceRegistrationState** 和 **managementAgent** 属性。|
|更改|beta|向 [mobileAppCategory](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcategory) 实体添加了 **lastModifiedDateTime** 属性。|
|更改|beta|向 [notificationMessageTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_notification_notificationmessagetemplate) 实体添加了 **brandingOptions**、**defaultLocale**、**displayName**、**fromEmailAddress**、**lastModifiedDateTime** 和 **localizedNotificationMessages** 属性。|
|更改|beta|向 [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) 实体添加了 **appsAllowTrustedAppsSideloading**、**appsBlockWindowsStoreOriginatedApps**、**developerUnlockSetting**、**edgeBlockAccessToAboutFlags**、**edgeBlockDeveloperTools**、**edgeBlockExtensions**、**edgeBlockInPrivateBrowsing**、**edgeFirstRunUrl**、**edgeHomepageUrls**、**gameDvrBlocked**、**settingsBlockAddProvisioningPackage**、**settingsBlockChangeLanguage**、**settingsBlockChangePowerSleep**、**settingsBlockChangeRegion**、**settingsBlockChangeSystemTime**、**settingsBlockEditDeviceName**、**settingsBlockRemoveProvisioningPackage**、**sharedUserAppDataAllowed**、**smartScreenBlockPromptOverride**、**smartScreenBlockPromptOverrideForFiles**、**storageRestrictAppDataToSystemVolume** 、**storageRestrictAppInstallToSystemVolume** 、**webRtcBlockLocalhostIpAddress**、**windowsStoreBlockAutoUpdate** 和 **windowsStoreEnablePrivateStoreOnly** 属性。|

## <a name="december-2016"></a>2016 年 12 月

### <a name="delta-query"></a>Delta 查询

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|Beta|将新的 delta 函数添加到以下实体，以执行[delta 查询](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_overview)：<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>有关示例，请参阅以下文章：<br/>
  [获取组的增量更改（预览）](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_groups)<br/>
  [获取文件夹中邮件的增量更改（预览）](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_messages)<br/>
  [获取用户的增量更改（预览）](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_users)|

### <a name="excel-apis"></a>Excel API

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|v1.0|添加了 workbookPivotTable 资源；数据透视表上的 refresh 和 refreshAll 操作；workbookRangeView 资源；已筛选的范围上的 visibleView 操作，可向用户返回 workbookRangeView；从 visibleView 中删除了 rows 集合和 range 资源；从 range 资源中删除了 columnsAfter、columnsBefore、resizedRange、rowsAbove、rowsBelow 函数；新增表属性。|

### <a name="intune-apis"></a>Intune API

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|Beta|添加了 Microsoft Intune 的资源和方法 API。这是用于支持 Intune 在 Azure Portal 上的公开预览的大型资源和方法集。有关 Intune 服务的信息，请参阅 [Intune 文档](https://go.microsoft.com/fwlink/?linkid=836405)。有关 Intune 资源和 API 的信息，请参阅[在 Microsoft Graph 中使用 Intune](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_graph_overview)。|

## <a name="october-2016"></a>2016 年 10 月

### <a name="authorization-provider"></a>授权提供程序

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|v1.0 和 beta|v2.0 授权终结点现在支持 client_credentials OAuth 授权哪些添加项可以用于[业务方案中的守护程序和长时间运行的进程](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-client-creds/)。|
|添加项|v1.0 和 beta|v2.0 授权终结点现在通过[管理员同意终结点](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#admin-restricted-scopes)支持[需要征得管理员同意的权限范围](http://developer.microsoft.com/en-us/graph/docs/concepts/permissions_reference)。|
|添加项|v1.0 和 beta|v2.0 授权终结点现在通过[管理员同意终结点](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#admin-restricted-scopes)支持对租户中的所有用户授予管理员同意。|

### <a name="invitation-apis"></a>邀请 API

|**更改类型**|**版本**|**说明**|
|:-------------|:-----------|:--------------|
|添加项|Beta|向邀请实体类型添加了 invitedUserType 属性，用于定义受邀用户类型（**来宾**或**成员**）。|
|删除|Beta|我们将于 2016 年11 月 11 日删除邀请实体类型中的 invitedToGroups 属性。这意味着，你将无法再使用此 API 将邀请的用户添加到组。而应使用[添加成员 API](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/group_post_members) 将用户添加到组。|

## <a name="september-2016"></a>2016 年 9 月

### <a name="azure-ad-application-proxy"></a>Azure AD 应用程序代理

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|现在可以在 Microsoft Graph 试用版终结点中使用 Azure AD 应用程序代理 API。这些 API 支持通过将 Azure AD 作为进行访问的通用控制面，安全地将本地应用程序发布给企业网络外部的用户。你可以使用已发布的 API 编写可以检索和更新应用程序代理的各个方面（例如，应用程序的 connectors、connectorGroups 和 onPremisesPublishing 设置）的应用程序。|

### <a name="drive"></a>驱动器

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|添加了 shared 集合以允许按 shareId 或共享 URL 访问共享的 driveItem。|
|添加项|Beta|向驱动器添加了 _search_ 函数，允许搜索驱动器根文件夹之外的更多项。|


### <a name="driveitem"></a>DriveItem

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|添加了对 createUploadSession 的支持，可允许将大于 4 MB 的文件上载到 OneDrive、OneDrive for Business 和 SharePoint 文档库。|
|添加项|Beta|向 driveItem 添加了 sharepointIds 属性，可返回 SharePoint 中存储的 driveItem 的传统 SharePoint API 标识符。|
|添加项|Beta|在 remoteItem 上添加了其他属性。|
|添加项|Beta|为 OneDrive for Business 中的文件添加了 quickXorHash 值。|
|添加项|Beta|添加了 createSharingLink 的作用域以允许创建企业共享链接或匿名共享链接。|

### <a name="extended-properties"></a>扩展属性

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|目前以下资源支持[扩展属性](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/extended-properties-overview)：message、mailFolder、event、calendar、contact、contactFolder、group event、group calendar、group post。|

### <a name="groups"></a>组

通过公共预览 API 添加了对动态组成员身份的支持，包括下表中列出的添加项。

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|添加了 **membershipRule** 属性，如果此组是动态组，则该属性会包含控制该组的成员资格的规则。|
|添加项|Beta|添加了 **membershipRuleProcessingState** 属性以控制是否对该组启用或暂停动态组成员资格处理。|
|添加项|Beta|设置了 **groupTypes** 属性以包含**“DynamicMembership”**来表明该组的动态组功能。|
|添加项|Beta|添加了 **preferredLanguage** 属性以指示 Office 365 组的首选语言。|
|添加项|Beta|添加了 **theme** 属性以指定 Office 365 组的颜色主题。|

### <a name="hybrid-deployment-support"></a>混合部署支持

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|应用可以使用 v1.0 Outlook 邮件、日历和联系人 API 访问使用 Exchange 2016 累积更新 3 (CU3) 的混合部署中的本地邮箱。可在特定的[混合部署](https://developer.microsoft.com/en-us/graph/docs/overview/hybrid_rest_support)中查找有关 REST API 支持的更多详细信息。**注意：**如果正在 v1.0 中使用这些 API 集，现在会发现应用（包括生产应用）可用于符合特定混合部署要求的本地邮箱。此功能仅在预览中可用。|

### <a name="identityriskevents"></a>IdentityRiskEvents

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|更改|Beta|作为架构更改的一部分，两个位置属性的类型将在 identityRiskEvents 终结点中替换为新的复杂类型，将在 identityRiskEvents 终结点中更改/添加以下属性：</br>**location** 已从 Edm.String 更改为 ComplexType signInLocation。<br/>**previousLocation** 已从 Edm.String 更改为 ComplexType signInLocation。<br/>**signInLocation** 是新的 ComplexType，其中包含 city、state、countryOrRegion 和 geoCoordinates 属性。<br/>**geoCoordinates** 是新的 ComplexType，其中包含 latitude 和 longitude 属性。|

### <a name="invitation-manager"></a>邀请管理器

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|现在可以在 Microsoft Graph 测试版终结点中使用邀请管理器 API。你可以使用邀请管理器 API 来创建一个邀请，以将外部用户添加到组织。作为邀请的一部分，还可以选择将受邀用户添加到 Office 365 组中。有关详细信息，请参阅[邀请管理器](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/invitation)。|

### <a name="onedrive"></a>OneDrive

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|在 **driveItem** 上添加了 **CreateUploadSession** 方法，可支持大型文件和可恢复上载。|
|添加项|v1.0|在 SharePoint 中的项目上添加了用于跟踪 SharePoint ID 的属性 (**sharepointIds**) 以及用于标识根文件夹的属性 (**root**)。|
|添加项|v1.0|添加了 **Shares** 根集合，可与 shareId 或共享链接一起使用来访问 OneDrive 和 SharePoint 中的共享项。它可返回新类型，即 sharedDriveItem。|
|添加项|v1.0|在 driveItem 上添加了 **Invite** 方法，可允许向项目添加权限。 |
|添加项|v1.0|在驱动器上添加了 **Search** 方法，可允许搜索驱动器中的项目和共享项目。 |
|添加项|v1.0|在哈希复杂类型上的文件复杂类型 quickXorHash 属性上添加了 **processingMetadata** 属性。 |
|添加项|v1.0|在哈希复杂类型上添加了 **quickXorHash** 属性 |

### <a name="outlook-calendar"></a>Outlook 日历

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|向 [event](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/event) 资源添加了 **onlineMeetingUrl** 属性。|
|添加项|Beta|向事件资源添加了 [forward](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/event_forward) 操作。|
|添加项|Beta|向[日历](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/calendar)资源添加了以下属性以支持日历共享：**canEdit**、**canShare**、**canViewPrivateItems**、**isShared**、**isShareWithMe** 和 **owner**。|

### <a name="outlook-mail"></a>Outlook 邮件

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|添加了 [mailboxSettings](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/mailboxsettings) 复杂类型，其中包括 **automaticRepliesSetting**、**timeZone** 和 **language** 属性。|
|添加项|v1.0|向 [user](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user) 资源添加了 **mailboxSettings** 属性。|
|添加项|Beta|支持在邮件中创建、列出、获取和删除一个或多个[提及](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/mention)实例。“提及”支持在邮件中进行呼叫以获得其他用户的关注。|
|添加项|Beta|添加了对 [getMailTips](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_getmailtips) 操作的支持，以便为特定收件人获取任何邮件提示。添加了以下资源：automaticRepliesMailTips、mailTips 和 mailTipsError。|

### <a name="query-parameters"></a>查询参数

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|更改|Beta|自 2016 年 9 月 26 日起，支持不含 $ 前缀的查询参数。在查询参数中，$ 前缀是可选的。有关详细信息，请参阅[在 Microsoft Graph 中支持不含 $ 前缀的查询参数](http://dev.office.com/queryparametersinMicrosoftGraph)博客文章。|

### <a name="sharepoint"></a>SharePoint

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|
  [按照 ID](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/list_get) 或[路径/URL](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/baseitem_getbyurl) 访问 SharePoint 网站和列表。|
|添加项|Beta|支持[列出、创建、获取和删除 listItem 实例](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/listitem)。|

### <a name="users"></a>用户

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|添加了 **refreshTokensValidFromDateTime** 只读属性，以指示刷新或会话令牌从何时开始生效。在该时间之前颁发的任何令牌均无效，且尝试使用此类令牌的任何行为将强制用户重新登录。|
|添加项|Beta|添加了 **showInAddressList** 属性来控制 Outlook 全局地址列表是否应包含此用户。|
|添加项|Beta|添加了 **invalidateAllRefreshTokens** 服务操作，可通过将 **refreshTokensValidFromDateTime** 用户属性重置为当前的日期时间来使向应用程序颁发的用户的所有刷新和会话令牌失效。|


### <a name="webhooks"></a>Webhook

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|将驱动器根项作为可供订阅的资源添加到了 Webhook。|

## <a name="august-2016"></a>2016 年 8 月

### <a name="contacts"></a>联系人

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|作为删除一些属性并将相应的集合添加到联系人终结点的架构更改的一部分，已将以下属性添加到联系人终结点：_Websites Collection(ComplexType:Website)_、_Phones Collection (ComplexType:Phone)_、_PostalAddress Collection(ComplexType:PhysicalAddress)_。有关详细信息，请参阅[即将对联系人和人员 API 做出的更改](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/)博客文章。|
|删除|Beta|作为删除一些属性并将相应的集合添加到联系人终结点的架构更改的一部分，已将以下属性从联系人终结点删除：BusinessHomePage、HomePhones、MobilePhone1、BusinessPhones、HomeAddress、BusinessAddress、OtherAddress。有关详细信息，请参阅[即将对联系人和人员 API 做出的更改](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/)博客文章。|

### <a name="excel-apis"></a>Excel API

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|Microsoft Graph 上的 Excel REST API 已公开发布。现在可以使用 Office 365 中的 Excel 工作簿构建广泛深入的集成。有关详细信息，请参阅[在 Microsoft Graph 上使用新的 Excel REST API 增强你的应用](http://dev.office.com/blogs/power-your-apps-with-the-new-excel-rest-api)博客文章。|

### <a name="people"></a>人员

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|更改|Beta|属性 WebSite 重命名为 Websites。有关详细信息，请参阅[即将对联系人和人员 API 做出的更改](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/)。|

### <a name="privileged-identity-management"></a>Privileged Identity Management

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|现在可以在 Microsoft Graph 测试版终结点中使用 Privileged Identity Management (PIM) REST API。[Privileged Identity Management](https://azure.microsoft.com/en-us/documentation/articles/active-directory-privileged-identity-management-configure/) 为全局管理员、帐务管理员等特权 Azure AD 组织角色提供及时的激活功能。可以使用已发布的 API 编写应用程序来检索和更新特权角色分配并激活用户角色。有关详细信息，请参阅 [Microsoft Graph：Azure AD Privileged Identity Management 预览 API 现在提供 Beta 版](http://dev.office.com/blogs/microsoft-graph-azure-ad-privileged-identity-management-apis-beta)和 [Azure AD Privileged Identity Management](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/privilegedidentitymanagement_root)。|

## <a name="july-2016"></a>2016 年 7 月

### <a name="administrative-units"></a>管理单元

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|引入新的管理单元预览 API。管理单元允许组织细分其 Azure Active Directory，并向这些细分项委派管理职能。细分项可以代表区域、部门、成本中心等。现在可通过 Microsoft Graph API 对此进行管理。|

## <a name="june-2016"></a>2016 年 6 月

### <a name="identityriskevents"></a>IdentityRiskEvents

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|引入了新的 IdentityRiskEvents 预览 API。此 API 与 Azure Active Directory Identity Protection 协同工作。你可以使用它来查询 Identity Protection 生成的风险事件。有关详细信息，请参阅[向 Microsoft Graph 引入新的预览 API：IdentityRiskEvents](http://dev.office.com/blogs/identityriskevents-api-preview) 博客文章。

### <a name="subscriptions"></a>订阅

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|mail 和 contacts 订阅现在支持仅应用作用域。|

## <a name="may-2016"></a>2016 年 5 月

### <a name="calendar"></a>日历

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|重大更改|Beta|针对 findMeetingTimes API 的更改。有关详细信息，请参阅 [Microsoft Graph findMeetingTimes API 更新](http://dev.office.com/microsoft-graph-findmeetingtimes-api-update)博客文章。此更改于 2016 年 5 月 19 日生效。

### <a name="contact"></a>联系人

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|添加了 extensions，它是用以支持 OData v4 开放类型 openTypeExtension 的抽象类型。|

### <a name="directory"></a>目录

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|重大更改|Beta|将 settingTemplateId 重命名为 templateId。此更改将于 2016 年 5 月 19 日生效。|

### <a name="event"></a>事件

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|添加了 extensions，它是用以支持 OData v4 开放类型 openTypeExtension 的抽象类型。|

### <a name="eventmessages"></a>EventMessages

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|向 eventMessages 添加了 inferenceClassification 和 extensions。|
|添加项|Beta|向 eventMessageRequest 添加了 responseRequested。|

### <a name="messages"></a>邮件

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|向 messages 添加了 inferenceClassification 和 extensions。|
|添加项|Beta|向 contactFolder 添加了 wellknownname。|针对 findMeetingTimes API 的更改。有关详细信息，请参阅 [Microsoft Graph findMeetingTimes API 更新](http://dev.office.com/microsoft-graph-findmeetingtimes-api-update)博客文章。此更改将于 2016 年 5 月 19 日生效。|

### <a name="post"></a>文章

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|添加了 extensions，它是用以支持 OData v4 开放类型 openTypeExtension 的抽象类型。|

### <a name="user"></a>用户

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|添加了 inferenceClassification 资源类型。|
|添加项|Beta|向 mailboxsettings 添加了 timeZone。|
|添加项|Beta|向 _user_ 添加了 API _findMeetingTimes_to。|

## <a name="april-2016"></a>2016 年 4 月

### <a name="general"></a>常规

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0 和 Beta|添加了遵守 Accept-Encoding:gzip 的支持。|
|添加项|v1.0|添加了对展开路径中的转换段的支持。例如，“https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event”。|
|添加项|Beta|添加了对结构化属性的 PATCH 请求的支持。例如：“PATCH /me/mailboxSettings”。|
|添加项|Beta|Outlook 在某些情况下（例如，用户没有邮箱许可证或租户没有 Exchange Online 订阅）无法处理请求时，现在可将 Azure Active Directory 用作 /beta/users/id/photo 请求的回退。注意：此回退同时适用于 GET 和 PATCH。|
|添加项|Beta|添加了对展开路径中的转换段的支持。例如：“https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event”。|

### <a name="onedrive"></a>OneDrive

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|修补程序|v1.0|修复了出现 500 和“不支持的扩展属性类型”故障的 OneDrive createLink 请求问题。|

## <a name="march-2016"></a>2016 年 3 月

### <a name="calendar"></a>日历

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|添加了 singleValueExtendedProperties 和 multiValueExtendedProperties 属性。|
|添加项|Beta|向 _meetingTimeCandidate_ 添加了 _suggestionHint_ 属性。|
|添加项|Beta|向 location 添加了 locationUri 属性。|
|添加项|Beta|向 _physicalAddress_ 添加了_type_ 和 _postOfficeBox_。|
|更改|Beta|findMeetingTimes 现在采用了新参数 ReturnSuggestionHints。|
|更改|Beta|findMeetingTimes 现在返回 meetingTimeCandidate 的集合。|

### <a name="drive"></a>驱动器

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0 和 beta|添加了 recent 功能以列出登录用户最近使用的一组项目。此列表包含用户驱动器中的项目，以及他们可以从其他驱动器访问的项目。示例：GET /me/drive/recent。|
|添加项|v1.0 和 beta|添加了 sharedWithMe 功能以列出与当前用户共享的项目集。示例：GET /me/drive/sharedWithMe。|

### <a name="driveitem"></a>DriveItem

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0 和 beta|添加了 remoteItem 类型以提供指向其他驱动器中的项目的链接。|
|添加项|v1.0 和 beta|添加了 sharingInvitation 类型以提供此权限关联的任何共享邀请的详细信息。|
|添加项|v1.0 和 beta|添加了 delta 函数以跟踪针对驱动器中项的更改。示例：GET /me/drive/items/{item-id}/delta|
|添加项|v1.0 和 beta|添加了 copy，可在新父级下或使用新名称创建一个 driveItem 副本（包括任何子级）。示例：POST /me/drive/items/{item-id}/copy。|
|添加项|v1.0 和 beta|conflictBehavior 实例属性现在适用于 driveItem。|
|添加项|Beta|添加了 invite 功能以发送对现有项目的共享邀请。共享邀请创建唯一的共享链接并向包含共享链接的邀请的收件人发送电子邮件。示例：POST /drive/items/{item-id}/invite。

### <a name="event"></a>事件

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|添加了新属性 onlineMeetingUrl 和新方法 cancel。|

### <a name="event-messages"></a>事件消息

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|向 eventmessage 对象添加了 startDateTime、endDateTime、location、type、recurrence、isOutOfDate、conversationIndex、unsubscribe、unsubscribeData、unsubscribeEnabled 和 flag 属性。|
|添加项|Beta|添加了 singleValueExtendedProperties 和 multiValueExtendedProperties 属性。|
|添加项|Beta|添加了新方法 unsubscribe。|

### <a name="excel"></a>Excel

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|我们将添加新的 Excel REST API，可允许你读取和修改 Excel 工作簿中的数据。现在则可以构建智能应用，允许用户通过向数据提供见解来从存储在 Excel 工作簿中的内容获取价值。利用 Excel 的分析功能、创建表格和图表并提取视觉上吸引人的图表图像 - 这些操作均可在应用内执行。有关详细信息，请参阅 [在 Microsoft Graph 中使用 Excel](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/excel).|

### <a name="general"></a>常规

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0 和 beta|改进了解析租户别名和拒绝的 JWT (AAD) 令牌时出现的错误消息。|
|添加项|v1.0 和 beta|收到含有空持有者令牌的请求时，在 www-authenticate 标头中现在返回授权服务终结点的位置。|
|添加项|v1.0 和 beta|现已修复筛选实体的 id 属性的功能。示例：GET https://graph.microsoft.com/v1.0/users?$filter=id+eq+'x'<br/>以前，对服务操作和功能的任何 POST 请求都需要在操作或功能名称前加上 microsoft.graph 前缀。例如：POST https://graph.microsoft.com/v1.0/me/Microsoft.Graph.getMemberGroups。<br/>现在不再需要此前缀（但是仍可指定此前缀）。因此，以下请求现在同样有效：POST https://graph.microsoft.com/v1.0/me/getMemberGroups。|
|更改|Beta|清理了订阅属性名称。|
|添加项|Beta|我们为实体及其关联功能添加了发现（通过 _directorySettingTemplates_）和替代默认行为（通过在模板中创建 _setting_）的功能。最初提供这个唯一的模板是为了控制 Office 组的行为。|

### <a name="mail-folder"></a>邮件文件夹

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|添加了 wellKnownName 和 userConfigurations 属性。|
|添加项|Beta|添加了 singleValueExtendedProperties 和 multiValueExtendedProperties 属性|

### <a name="messages"></a>邮件

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|添加了 mobilePhone 属性。|
|Addition|v1.0 和 beta|添加了 internetMessageId 属性。由 [RFC2822](http://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。|
|更改|Beta|将 mobilePhone1 属性重命名为 mobilePhone。|
|更改|Beta|_createReply_ 和 _createReplyAll_ 采用了新参数：_Message_ 和 _comment_。|
|更改|Beta|_createForward_ 采用了新参数：_Message_、_ToRecipients_ 和 _comment_。|
|更改|Beta|_reply_、_replyAll_ 和 _forward_ 采用了新参数 _Message_。|

### <a name="permission"></a>权限

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0 和 beta|添加了 sharingInvitation 属性以提供此权限关联的任何共享邀请的详细信息。|

### <a name="person"></a>人员

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|添加了新属性：birthday、personNotes、isFavorite、phones、permission、postalAddresses、websites、yomiCompany、department、profession、mailboxType 和 personType。|
|Addition|Beta|添加了以下新枚举类型：_physicalAddressType_、_webSite_、_phone_ 和 _webSiteType_。|

### <a name="reference-attachment"></a>参考附件

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|添加了新属性：sourceUrl、providerType、thumbnailUrl、previewUrl、permission 和 isFolder。|
|Addition|Beta|添加了 singleValueExtendedProperties 和 multiValueExtendedProperties 属性。|
|添加项|Beta|添加了以下新枚举类型：_referenceAttachmentProvider_ 和 _referenceAttachmentPermission_。|

### <a name="subscriptions"></a>订阅

|**更改类型**|**终结点**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|Webhook 现在已在 V1.0 终结点上普遍可用，可通过 /Subscriptions 资源获取。创建、读取、续订和删除订阅以接收有关 Outlook 和 Office 365 组对话中数据的通知。|

### <a name="user"></a>用户

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|添加了 mailboxSettings 属性和相应的类型。|

## <a name="february-2016"></a>2016 年 2 月

### <a name="driveitem"></a>DriveItem

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0 和 beta|在 Microsoft 帐户的 driveItem 上添加了新的 remoteItem 属性。|

### <a name="general"></a>常规

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|更改|v1.0 和 beta|-/me/drive 现在同时适用于 Microsoft 帐户和工作及学校帐户。|
|更改|v1.0 和 beta|对按需预配其 OneDrive 存储的帐户的驱动器请求工作更为可靠，且适用于租户默认的 SharePoint 网站使用非标准名称的更多场景。|
|删除|Beta|删除了测试版架构中的各种未实现的类型，以便更加匹配 1.0 架构。|

### <a name="subscriptions"></a>订阅

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|订阅创建时的 notificationUrl 验证。有关详细信息，请参阅 [Microsoft Graph WebHook 更新 - 2016 年 1 月](http://dev.office.com/blogs/Microsoft-Graph-WebHooks-Update-January-2016)。|
|添加项|Beta|现在可删除订阅实体：DELETE https://graph.microsoft.com/beta/subscriptions/|

### <a name="users"></a>用户

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|更改|v1.0 和 beta|现在为 Microsoft 帐户返回 displayName。|

## <a name="january-2016"></a>2016 年 1 月

### <a name="contacts"></a>联系人

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|v1.0|向个人联系人实体集添加了 mobilePhone 属性。|

### <a name="directoryobjects"></a>directoryObjects

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|修补程序|v1.0 和 beta|修复了出现以下错误的绑定到 directoryObjects 的调用操作：操作中的返回类型不可用于给定的实体集。它适用于以下操作：_microsoft.graph.checkMemberObjects_、_microsoft.graph.getMemberObjects_、_microsoft.graph.checkMemberGroups_、_microsoft.graph.assignLicense_、_microsoft.graph.changePassword_。|

## <a name="december-2015"></a>2015 年 12 月

### <a name="contacts"></a>联系人

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|向个人联系人实体集添加了 mobilePhone 属性。|

### <a name="general"></a>常规

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|修补程序|v1.0 和 beta|修复了使用 $filter 表达式多次指定同一属性，会出现以下 500 错误的请求：已添加具有相同键的项目。|
|修补程序|v1.0 和 beta|修复了对操作参数名称和值不区分大小写的错误。|
|修补程序|v1.0 和 beta|修复了对包含某些嵌入复杂属性的 null 值的负载的请求处理出现 null 引用异常的问题。|
|Addition|v1.0 和 beta|添加了对复杂类型属性进行排序和筛选的支持。|
|Addition|v1.0 和 beta|在 401 响应上的 www-authenticate 标头中添加了 authorization_uri 属性。该 URL 可用于启动令牌获取流。|
|添加项|v1.0 和 beta|改进了用户和组中的错误消息。|

### <a name="groups"></a>组

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|修补程序|v1.0 和 beta|修复了无法调用以下组操作的问题：microsoft.graph.addFavorite、microsoft.graph.removeFavorite 和 microsoft.graph.resetUnseenCount。|

### <a name="messages"></a>邮件

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|添加项|Beta|向 eventMessage 类型添加了 eventMessage 的 eventMessageRequest 子类型以及 startDateTime endDateTime、location、type、recurrence 和 isOutOfDate 属性。|

### <a name="users"></a>用户

|**更改类型**|**版本**|**说明**|
|:--------------|:-----------|:--------------|
|修补程序|v1.0 和 beta|修复了通过用户主体名称 (UPN) 引用用户时可以选择其他用户上的某些用户属性的问题。例如：https://graph.microsoft.com/v1.0/users/anotherUser@contoso.com?$select=aboutMe|
|修补程序|v1.0 和 beta|修复了在调用 _microsoft.graph.reminderView_ 用户绑定功能时出现以下错误的问题：无法在类型 Microsoft.OutlookServices.Reminder 上找到名为 businessPhones 的属性。|
|修补程序|v1.0 和 beta|修复了出现 400 错误的用户创建和更新 (POST/PATCH /v1.0/users)。|
