---
title: 获取 windows10GeneralConfiguration
description: 读取 windows10GeneralConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b674f3f5c7f7c59a7f172980be63b1cf15c45007
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33920976"
---
# <a name="get-windows10generalconfiguration"></a><span data-ttu-id="e51e0-103">获取 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="e51e0-103">Get windows10GeneralConfiguration</span></span>

> <span data-ttu-id="e51e0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e51e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e51e0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e51e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e51e0-106">读取 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e51e0-106">Read properties and relationships of the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e51e0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e51e0-107">Prerequisites</span></span>
<span data-ttu-id="e51e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e51e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e51e0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e51e0-110">Permission type</span></span>|<span data-ttu-id="e51e0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e51e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e51e0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e51e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e51e0-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e51e0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e51e0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e51e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e51e0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e51e0-115">Not supported.</span></span>|
|<span data-ttu-id="e51e0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e51e0-116">Application</span></span>|<span data-ttu-id="e51e0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e51e0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e51e0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e51e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e51e0-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e51e0-119">Optional query parameters</span></span>
<span data-ttu-id="e51e0-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e51e0-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e51e0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e51e0-121">Request headers</span></span>
|<span data-ttu-id="e51e0-122">标头</span><span class="sxs-lookup"><span data-stu-id="e51e0-122">Header</span></span>|<span data-ttu-id="e51e0-123">值</span><span class="sxs-lookup"><span data-stu-id="e51e0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e51e0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e51e0-124">Authorization</span></span>|<span data-ttu-id="e51e0-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e51e0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e51e0-126">接受</span><span class="sxs-lookup"><span data-stu-id="e51e0-126">Accept</span></span>|<span data-ttu-id="e51e0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e51e0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e51e0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e51e0-128">Request body</span></span>
<span data-ttu-id="e51e0-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e51e0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e51e0-130">响应</span><span class="sxs-lookup"><span data-stu-id="e51e0-130">Response</span></span>
<span data-ttu-id="e51e0-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e51e0-131">If successful, this method returns a `200 OK` response code and [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e51e0-132">示例</span><span class="sxs-lookup"><span data-stu-id="e51e0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e51e0-133">请求</span><span class="sxs-lookup"><span data-stu-id="e51e0-133">Request</span></span>
<span data-ttu-id="e51e0-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e51e0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e51e0-135">响应</span><span class="sxs-lookup"><span data-stu-id="e51e0-135">Response</span></span>
<span data-ttu-id="e51e0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e51e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 14347

{
  "value": {
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
    "authenticationWebSignIn": "enabled",
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
    "edgeKioskModeRestriction": "digitalSignage",
    "edgeKioskResetAfterIdleTimeInMinutes": 4,
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
    "defenderScheduleScanEnableLowCpuPriority": true,
    "defenderDisableCatchupQuickScan": true,
    "defenderDisableCatchupFullScan": true,
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
    "privacyDisableLaunchExperience": true,
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
    "edgeBlockSearchEngineCustomization": true,
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
    "dataProtectionBlockDirectMemoryAccess": true,
    "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
      "App Management Package Family Names To Launch After Log On value"
    ]
  }
}
```




