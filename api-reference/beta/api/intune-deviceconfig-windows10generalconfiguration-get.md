---
title: 获取 windows10GeneralConfiguration
description: 读取 windows10GeneralConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a4b7690250862080e53fe5458e178a094672f2b6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947846"
---
# <a name="get-windows10generalconfiguration"></a><span data-ttu-id="688bd-103">获取 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="688bd-103">Get windows10GeneralConfiguration</span></span>

> <span data-ttu-id="688bd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="688bd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="688bd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="688bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="688bd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="688bd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="688bd-107">读取 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="688bd-107">Read properties and relationships of the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="688bd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="688bd-108">Prerequisites</span></span>
<span data-ttu-id="688bd-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="688bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="688bd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="688bd-111">Permission type</span></span>|<span data-ttu-id="688bd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="688bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="688bd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="688bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="688bd-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="688bd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="688bd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="688bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="688bd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="688bd-116">Not supported.</span></span>|
|<span data-ttu-id="688bd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="688bd-117">Application</span></span>|<span data-ttu-id="688bd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="688bd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="688bd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="688bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="688bd-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="688bd-120">Optional query parameters</span></span>
<span data-ttu-id="688bd-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="688bd-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="688bd-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="688bd-122">Request headers</span></span>
|<span data-ttu-id="688bd-123">标头</span><span class="sxs-lookup"><span data-stu-id="688bd-123">Header</span></span>|<span data-ttu-id="688bd-124">值</span><span class="sxs-lookup"><span data-stu-id="688bd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="688bd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="688bd-125">Authorization</span></span>|<span data-ttu-id="688bd-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="688bd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="688bd-127">Accept</span><span class="sxs-lookup"><span data-stu-id="688bd-127">Accept</span></span>|<span data-ttu-id="688bd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="688bd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="688bd-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="688bd-129">Request body</span></span>
<span data-ttu-id="688bd-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="688bd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="688bd-131">响应</span><span class="sxs-lookup"><span data-stu-id="688bd-131">Response</span></span>
<span data-ttu-id="688bd-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="688bd-132">If successful, this method returns a `200 OK` response code and [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="688bd-133">示例</span><span class="sxs-lookup"><span data-stu-id="688bd-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="688bd-134">请求</span><span class="sxs-lookup"><span data-stu-id="688bd-134">Request</span></span>
<span data-ttu-id="688bd-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="688bd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="688bd-136">响应</span><span class="sxs-lookup"><span data-stu-id="688bd-136">Response</span></span>
<span data-ttu-id="688bd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="688bd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 12903

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
    "windows10AppsForceUpdateSchedule": {
      "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "recurrence": "daily",
      "runImmediatelyIfAfterStartDateTime": true
    },
    "enableAutomaticRedeployment": true,
    "assignedAccessSingleModeUserName": "Assigned Access Single Mode User Name value",
    "assignedAccessSingleModeAppUserModelId": "Assigned Access Single Mode App User Model Id value",
    "microsoftAccountSignInAssistantSettings": "disabled",
    "authenticationAllowSecondaryDevice": true,
    "authenticationAllowFIDODevice": true,
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
}
```





