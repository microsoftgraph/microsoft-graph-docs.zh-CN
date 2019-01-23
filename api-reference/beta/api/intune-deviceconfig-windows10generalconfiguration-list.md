---
title: 列出 windows10GeneralConfigurations
description: 列出 windows10GeneralConfiguration 对象的属性和关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 256fd9de47d91be93c7b6fb24c15397b4cc17aa5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411958"
---
# <a name="list-windows10generalconfigurations"></a>列出 windows10GeneralConfigurations

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

列出 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的属性和关系。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 14497

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
      "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "taskManagerBlockEndTask": true,
      "windows10AppsForceUpdateSchedule": {
        "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
        "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
        "recurrence": "daily",
        "runImmediatelyIfAfterStartDateTime": true
      },
      "enableAutomaticRedeployment": true,
      "microsoftAccountSignInAssistantSettings": "disabled",
      "authenticationAllowSecondaryDevice": true,
      "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
      "cryptographyAllowFipsAlgorithmPolicy": true,
      "displayAppListWithGdiDPIScalingTurnedOn": [
        "Display App List With Gdi DPIScaling Turned On value"
      ],
      "displayAppListWithGdiDPIScalingTurnedOff": [
        "Display App List With Gdi DPIScaling Turned Off value"
      ],
      "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
      "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
      "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
      "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
      "enterpriseCloudPrintDiscoveryMaxLimit": 5,
      "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
      "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
      "messagingBlockSync": true,
      "messagingBlockMMS": true,
      "messagingBlockRichCommunicationServices": true,
      "printerNames": [
        "Printer Names value"
      ],
      "printerDefaultName": "Printer Default Name value",
      "printerBlockAddition": true,
      "searchBlockDiacritics": true,
      "searchDisableAutoLanguageDetection": true,
      "searchDisableIndexingEncryptedItems": true,
      "searchEnableRemoteQueries": true,
      "searchDisableUseLocation": true,
      "searchDisableLocation": true,
      "searchDisableIndexerBackoff": true,
      "searchDisableIndexingRemovableDrive": true,
      "searchEnableAutomaticIndexSizeManangement": true,
      "searchBlockWebResults": true,
      "securityBlockAzureADJoinedDevicesAutoEncryption": true,
      "diagnosticsDataSubmissionMode": "none",
      "oneDriveDisableFileSync": true,
      "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
      "edgeTelemetryForMicrosoft365Analytics": "intranet",
      "inkWorkspaceAccess": "enabled",
      "inkWorkspaceAccessState": "blocked",
      "inkWorkspaceBlockSuggestedApps": true,
      "smartScreenEnableAppInstallControl": true,
      "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
      "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
      "bluetoothAllowedServices": [
        "Bluetooth Allowed Services value"
      ],
      "bluetoothBlockAdvertising": true,
      "bluetoothBlockPromptedProximalConnections": true,
      "bluetoothBlockDiscoverableMode": true,
      "bluetoothBlockPrePairing": true,
      "edgeBlockAutofill": true,
      "edgeBlocked": true,
      "edgeCookiePolicy": "allow",
      "edgeBlockDeveloperTools": true,
      "edgeBlockSendingDoNotTrackHeader": true,
      "edgeBlockExtensions": true,
      "edgeBlockInPrivateBrowsing": true,
      "edgeBlockJavaScript": true,
      "edgeBlockPasswordManager": true,
      "edgeBlockAddressBarDropdown": true,
      "edgeBlockCompatibilityList": true,
      "edgeClearBrowsingDataOnExit": true,
      "edgeAllowStartPagesModification": true,
      "edgeDisableFirstRunPage": true,
      "edgeBlockLiveTileDataCollection": true,
      "edgeSyncFavoritesWithInternetExplorer": true,
      "edgeFavoritesListLocation": "Edge Favorites List Location value",
      "edgeBlockEditFavorites": true,
      "edgeNewTabPageURL": "Edge New Tab Page URL value",
      "edgeHomeButtonConfiguration": {
        "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
      },
      "edgeHomeButtonConfigurationEnabled": true,
      "edgeOpensWith": "startPage",
      "edgeBlockSideloadingExtensions": true,
      "edgeRequiredExtensionPackageFamilyNames": [
        "Edge Required Extension Package Family Names value"
      ],
      "edgeBlockPrinting": true,
      "edgeFavoritesBarVisibility": "hide",
      "edgeBlockSavingHistory": true,
      "edgeBlockFullScreenMode": true,
      "edgeBlockWebContentOnNewTabPage": true,
      "edgeBlockTabPreloading": true,
      "edgeBlockPrelaunch": true,
      "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
      "edgePreventCertificateErrorOverride": true,
      "cellularBlockDataWhenRoaming": true,
      "cellularBlockVpn": true,
      "cellularBlockVpnWhenRoaming": true,
      "cellularData": "required",
      "defenderBlockEndUserAccess": true,
      "defenderDaysBeforeDeletingQuarantinedMalware": 12,
      "defenderDetectedMalwareActions": {
        "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
        "lowSeverity": "clean",
        "moderateSeverity": "clean",
        "highSeverity": "clean",
        "severeSeverity": "clean"
      },
      "defenderSystemScanSchedule": "everyday",
      "defenderFilesAndFoldersToExclude": [
        "Defender Files And Folders To Exclude value"
      ],
      "defenderFileExtensionsToExclude": [
        "Defender File Extensions To Exclude value"
      ],
      "defenderScanMaxCpu": 2,
      "defenderMonitorFileActivity": "disable",
      "defenderPotentiallyUnwantedAppAction": "block",
      "defenderPotentiallyUnwantedAppActionSetting": "enable",
      "defenderProcessesToExclude": [
        "Defender Processes To Exclude value"
      ],
      "defenderPromptForSampleSubmission": "alwaysPrompt",
      "defenderRequireBehaviorMonitoring": true,
      "defenderRequireCloudProtection": true,
      "defenderRequireNetworkInspectionSystem": true,
      "defenderRequireRealTimeMonitoring": true,
      "defenderScanArchiveFiles": true,
      "defenderScanDownloads": true,
      "defenderScanNetworkFiles": true,
      "defenderScanIncomingMail": true,
      "defenderScanMappedNetworkDrivesDuringFullScan": true,
      "defenderScanRemovableDrivesDuringFullScan": true,
      "defenderScanScriptsLoadedInInternetExplorer": true,
      "defenderSignatureUpdateIntervalInHours": 6,
      "defenderScanType": "disabled",
      "defenderScheduledScanTime": "11:59:10.9990000",
      "defenderScheduledQuickScanTime": "11:58:49.3840000",
      "defenderCloudBlockLevel": "high",
      "defenderCloudExtendedTimeout": 12,
      "defenderCloudExtendedTimeoutInSeconds": 5,
      "defenderBlockOnAccessProtection": true,
      "defenderScheduleScanDay": "monday",
      "defenderSubmitSamplesConsentType": "alwaysPrompt",
      "lockScreenAllowTimeoutConfiguration": true,
      "lockScreenBlockActionCenterNotifications": true,
      "lockScreenBlockCortana": true,
      "lockScreenBlockToastNotifications": true,
      "lockScreenTimeoutInSeconds": 10,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordMinimumCharacterSetCount": 0,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequired": true,
      "passwordRequireWhenResumeFromIdleState": true,
      "passwordRequiredType": "alphanumeric",
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordMinimumAgeInDays": 8,
      "privacyAdvertisingId": "blocked",
      "privacyAutoAcceptPairingAndConsentPrompts": true,
      "privacyBlockInputPersonalization": true,
      "privacyBlockPublishUserActivities": true,
      "privacyBlockActivityFeed": true,
      "startBlockUnpinningAppsFromTaskbar": true,
      "startMenuAppListVisibility": "collapse",
      "startMenuHideChangeAccountSettings": true,
      "startMenuHideFrequentlyUsedApps": true,
      "startMenuHideHibernate": true,
      "startMenuHideLock": true,
      "startMenuHidePowerButton": true,
      "startMenuHideRecentJumpLists": true,
      "startMenuHideRecentlyAddedApps": true,
      "startMenuHideRestartOptions": true,
      "startMenuHideShutDown": true,
      "startMenuHideSignOut": true,
      "startMenuHideSleep": true,
      "startMenuHideSwitchAccount": true,
      "startMenuHideUserTile": true,
      "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
      "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
      "startMenuMode": "fullScreen",
      "startMenuPinnedFolderDocuments": "hide",
      "startMenuPinnedFolderDownloads": "hide",
      "startMenuPinnedFolderFileExplorer": "hide",
      "startMenuPinnedFolderHomeGroup": "hide",
      "startMenuPinnedFolderMusic": "hide",
      "startMenuPinnedFolderNetwork": "hide",
      "startMenuPinnedFolderPersonalFolder": "hide",
      "startMenuPinnedFolderPictures": "hide",
      "startMenuPinnedFolderSettings": "hide",
      "startMenuPinnedFolderVideos": "hide",
      "settingsBlockSettingsApp": true,
      "settingsBlockSystemPage": true,
      "settingsBlockDevicesPage": true,
      "settingsBlockNetworkInternetPage": true,
      "settingsBlockPersonalizationPage": true,
      "settingsBlockAccountsPage": true,
      "settingsBlockTimeLanguagePage": true,
      "settingsBlockEaseOfAccessPage": true,
      "settingsBlockPrivacyPage": true,
      "settingsBlockUpdateSecurityPage": true,
      "settingsBlockAppsPage": true,
      "settingsBlockGamingPage": true,
      "windowsSpotlightBlockConsumerSpecificFeatures": true,
      "windowsSpotlightBlocked": true,
      "windowsSpotlightBlockOnActionCenter": true,
      "windowsSpotlightBlockTailoredExperiences": true,
      "windowsSpotlightBlockThirdPartyNotifications": true,
      "windowsSpotlightBlockWelcomeExperience": true,
      "windowsSpotlightBlockWindowsTips": true,
      "windowsSpotlightConfigureOnLockScreen": "disabled",
      "networkProxyApplySettingsDeviceWide": true,
      "networkProxyDisableAutoDetect": true,
      "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
      "networkProxyServer": {
        "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
        "address": "Address value",
        "exceptions": [
          "Exceptions value"
        ],
        "useForLocalAddresses": true
      },
      "accountsBlockAddingNonMicrosoftAccountEmail": true,
      "antiTheftModeBlocked": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "connectedDevicesServiceBlocked": true,
      "certificatesBlockManualRootCertificateInstallation": true,
      "copyPasteBlocked": true,
      "cortanaBlocked": true,
      "deviceManagementBlockFactoryResetOnMobile": true,
      "deviceManagementBlockManualUnenroll": true,
      "safeSearchFilter": "strict",
      "edgeBlockPopups": true,
      "edgeBlockSearchSuggestions": true,
      "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
      "edgeSendIntranetTrafficToInternetExplorer": true,
      "edgeRequireSmartScreen": true,
      "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
      "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
      "edgeSearchEngine": {
        "@odata.type": "microsoft.graph.edgeSearchEngineBase"
      },
      "edgeHomepageUrls": [
        "Edge Homepage Urls value"
      ],
      "edgeBlockAccessToAboutFlags": true,
      "smartScreenBlockPromptOverride": true,
      "smartScreenBlockPromptOverrideForFiles": true,
      "webRtcBlockLocalhostIpAddress": true,
      "internetSharingBlocked": true,
      "settingsBlockAddProvisioningPackage": true,
      "settingsBlockRemoveProvisioningPackage": true,
      "settingsBlockChangeSystemTime": true,
      "settingsBlockEditDeviceName": true,
      "settingsBlockChangeRegion": true,
      "settingsBlockChangeLanguage": true,
      "settingsBlockChangePowerSleep": true,
      "locationServicesBlocked": true,
      "microsoftAccountBlocked": true,
      "microsoftAccountBlockSettingsSync": true,
      "nfcBlocked": true,
      "resetProtectionModeBlocked": true,
      "screenCaptureBlocked": true,
      "storageBlockRemovableStorage": true,
      "storageRequireMobileDeviceEncryption": true,
      "usbBlocked": true,
      "voiceRecordingBlocked": true,
      "wiFiBlockAutomaticConnectHotspots": true,
      "wiFiBlocked": true,
      "wiFiBlockManualConfiguration": true,
      "wiFiScanInterval": 0,
      "wirelessDisplayBlockProjectionToThisDevice": true,
      "wirelessDisplayBlockUserInputFromReceiver": true,
      "wirelessDisplayRequirePinForPairing": true,
      "windowsStoreBlocked": true,
      "appsAllowTrustedAppsSideloading": "blocked",
      "windowsStoreBlockAutoUpdate": true,
      "developerUnlockSetting": "blocked",
      "sharedUserAppDataAllowed": true,
      "appsBlockWindowsStoreOriginatedApps": true,
      "windowsStoreEnablePrivateStoreOnly": true,
      "storageRestrictAppDataToSystemVolume": true,
      "storageRestrictAppInstallToSystemVolume": true,
      "gameDvrBlocked": true,
      "experienceBlockDeviceDiscovery": true,
      "experienceBlockErrorDialogWhenNoSIM": true,
      "experienceBlockTaskSwitcher": true,
      "logonBlockFastUserSwitching": true,
      "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
      "appManagementMSIAllowUserControlOverInstall": true,
      "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
      "dataProtectionBlockDirectMemoryAccess": true
    }
  ]
}
```




