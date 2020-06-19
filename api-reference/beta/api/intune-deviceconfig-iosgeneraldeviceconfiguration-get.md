---
title: 获取 iosGeneralDeviceConfiguration
description: 读取 iosGeneralDeviceConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 62509d7ffb50cd33719bc33ea1139703d740be5e
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792812"
---
# <a name="get-iosgeneraldeviceconfiguration"></a><span data-ttu-id="e458d-103">获取 iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e458d-103">Get iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="e458d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e458d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e458d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e458d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e458d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e458d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e458d-107">读取 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e458d-107">Read properties and relationships of the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e458d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e458d-108">Prerequisites</span></span>
<span data-ttu-id="e458d-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e458d-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e458d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e458d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e458d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e458d-111">Permission type</span></span>|<span data-ttu-id="e458d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e458d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e458d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e458d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e458d-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e458d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e458d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e458d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e458d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e458d-116">Not supported.</span></span>|
|<span data-ttu-id="e458d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e458d-117">Application</span></span>|<span data-ttu-id="e458d-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e458d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e458d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e458d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e458d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e458d-120">Optional query parameters</span></span>
<span data-ttu-id="e458d-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e458d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e458d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e458d-122">Request headers</span></span>
|<span data-ttu-id="e458d-123">标头</span><span class="sxs-lookup"><span data-stu-id="e458d-123">Header</span></span>|<span data-ttu-id="e458d-124">值</span><span class="sxs-lookup"><span data-stu-id="e458d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e458d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e458d-125">Authorization</span></span>|<span data-ttu-id="e458d-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e458d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e458d-127">接受</span><span class="sxs-lookup"><span data-stu-id="e458d-127">Accept</span></span>|<span data-ttu-id="e458d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e458d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e458d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e458d-129">Request body</span></span>
<span data-ttu-id="e458d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e458d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e458d-131">响应</span><span class="sxs-lookup"><span data-stu-id="e458d-131">Response</span></span>
<span data-ttu-id="e458d-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e458d-132">If successful, this method returns a `200 OK` response code and [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e458d-133">示例</span><span class="sxs-lookup"><span data-stu-id="e458d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e458d-134">请求</span><span class="sxs-lookup"><span data-stu-id="e458d-134">Request</span></span>
<span data-ttu-id="e458d-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e458d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e458d-136">响应</span><span class="sxs-lookup"><span data-stu-id="e458d-136">Response</span></span>
<span data-ttu-id="e458d-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e458d-137">Here is an example of the response.</span></span> <span data-ttu-id="e458d-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e458d-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e458d-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e458d-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 11336

{
  "value": {
    "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
    "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "deviceManagementApplicabilityRuleOsEdition": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
      "osEditionTypes": [
        "windows10EnterpriseN"
      ],
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleOsVersion": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
      "minOSVersion": "Min OSVersion value",
      "maxOSVersion": "Max OSVersion value",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleDeviceMode": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
      "deviceMode": "sModeConfiguration",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "accountBlockModification": true,
    "activationLockAllowWhenSupervised": true,
    "airDropBlocked": true,
    "airDropForceUnmanagedDropTarget": true,
    "airPlayForcePairingPasswordForOutgoingRequests": true,
    "appleWatchBlockPairing": true,
    "appleWatchForceWristDetection": true,
    "appleNewsBlocked": true,
    "appsSingleAppModeList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "appsVisibilityList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "appsVisibilityListType": "appsInListCompliant",
    "appStoreBlockAutomaticDownloads": true,
    "appStoreBlocked": true,
    "appStoreBlockInAppPurchases": true,
    "appStoreBlockUIAppInstallation": true,
    "appStoreRequirePassword": true,
    "autoFillForceAuthentication": true,
    "bluetoothBlockModification": true,
    "cameraBlocked": true,
    "cellularBlockDataRoaming": true,
    "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
    "cellularBlockPerAppDataModification": true,
    "cellularBlockPersonalHotspot": true,
    "cellularBlockPlanModification": true,
    "cellularBlockVoiceRoaming": true,
    "certificatesBlockUntrustedTlsCertificates": true,
    "classroomAppBlockRemoteScreenObservation": true,
    "classroomAppForceUnpromptedScreenObservation": true,
    "classroomForceAutomaticallyJoinClasses": true,
    "classroomForceUnpromptedAppAndDeviceLock": true,
    "compliantAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "compliantAppListType": "appsInListCompliant",
    "configurationProfileBlockChanges": true,
    "definitionLookupBlocked": true,
    "deviceBlockEnableRestrictions": true,
    "deviceBlockEraseContentAndSettings": true,
    "deviceBlockNameModification": true,
    "diagnosticDataBlockSubmission": true,
    "diagnosticDataBlockSubmissionModification": true,
    "documentsBlockManagedDocumentsInUnmanagedApps": true,
    "documentsBlockUnmanagedDocumentsInManagedApps": true,
    "emailInDomainSuffixes": [
      "Email In Domain Suffixes value"
    ],
    "enterpriseAppBlockTrust": true,
    "enterpriseAppBlockTrustModification": true,
    "esimBlockModification": true,
    "faceTimeBlocked": true,
    "findMyFriendsBlocked": true,
    "gamingBlockGameCenterFriends": true,
    "gamingBlockMultiplayer": true,
    "gameCenterBlocked": true,
    "hostPairingBlocked": true,
    "iBooksStoreBlocked": true,
    "iBooksStoreBlockErotica": true,
    "iCloudBlockActivityContinuation": true,
    "iCloudBlockBackup": true,
    "iCloudBlockDocumentSync": true,
    "iCloudBlockManagedAppsSync": true,
    "iCloudBlockPhotoLibrary": true,
    "iCloudBlockPhotoStreamSync": true,
    "iCloudBlockSharedPhotoStream": true,
    "iCloudRequireEncryptedBackup": true,
    "iTunesBlockExplicitContent": true,
    "iTunesBlockMusicService": true,
    "iTunesBlockRadio": true,
    "keyboardBlockAutoCorrect": true,
    "keyboardBlockDictation": true,
    "keyboardBlockPredictive": true,
    "keyboardBlockShortcuts": true,
    "keyboardBlockSpellCheck": true,
    "kioskModeAllowAssistiveSpeak": true,
    "kioskModeAllowAssistiveTouchSettings": true,
    "kioskModeAllowAutoLock": true,
    "kioskModeBlockAutoLock": true,
    "kioskModeAllowColorInversionSettings": true,
    "kioskModeAllowRingerSwitch": true,
    "kioskModeBlockRingerSwitch": true,
    "kioskModeAllowScreenRotation": true,
    "kioskModeBlockScreenRotation": true,
    "kioskModeAllowSleepButton": true,
    "kioskModeBlockSleepButton": true,
    "kioskModeAllowTouchscreen": true,
    "kioskModeBlockTouchscreen": true,
    "kioskModeEnableVoiceControl": true,
    "kioskModeAllowVoiceControlModification": true,
    "kioskModeAllowVoiceOverSettings": true,
    "kioskModeAllowVolumeButtons": true,
    "kioskModeBlockVolumeButtons": true,
    "kioskModeAllowZoomSettings": true,
    "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
    "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
    "kioskModeRequireAssistiveTouch": true,
    "kioskModeRequireColorInversion": true,
    "kioskModeRequireMonoAudio": true,
    "kioskModeRequireVoiceOver": true,
    "kioskModeRequireZoom": true,
    "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
    "lockScreenBlockControlCenter": true,
    "lockScreenBlockNotificationView": true,
    "lockScreenBlockPassbook": true,
    "lockScreenBlockTodayView": true,
    "mediaContentRatingAustralia": {
      "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingCanada": {
      "@odata.type": "microsoft.graph.mediaContentRatingCanada",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingFrance": {
      "@odata.type": "microsoft.graph.mediaContentRatingFrance",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingGermany": {
      "@odata.type": "microsoft.graph.mediaContentRatingGermany",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingIreland": {
      "@odata.type": "microsoft.graph.mediaContentRatingIreland",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingJapan": {
      "@odata.type": "microsoft.graph.mediaContentRatingJapan",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingNewZealand": {
      "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingUnitedKingdom": {
      "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingUnitedStates": {
      "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "networkUsageRules": [
      {
        "@odata.type": "microsoft.graph.iosNetworkUsageRule",
        "managedApps": [
          {
            "@odata.type": "microsoft.graph.appListItem",
            "name": "Name value",
            "publisher": "Publisher value",
            "appStoreUrl": "https://example.com/appStoreUrl/",
            "appId": "App Id value"
          }
        ],
        "cellularDataBlockWhenRoaming": true,
        "cellularDataBlocked": true
      }
    ],
    "mediaContentRatingApps": "allBlocked",
    "messagesBlocked": true,
    "notificationsBlockSettingsModification": true,
    "passcodeBlockFingerprintUnlock": true,
    "passcodeBlockFingerprintModification": true,
    "passcodeBlockModification": true,
    "passcodeBlockSimple": true,
    "passcodeExpirationDays": 6,
    "passcodeMinimumLength": 5,
    "passcodeMinutesOfInactivityBeforeLock": 5,
    "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
    "passcodeMinimumCharacterSetCount": 0,
    "passcodePreviousPasscodeBlockCount": 2,
    "passcodeSignInFailureCountBeforeWipe": 4,
    "passcodeRequiredType": "alphanumeric",
    "passcodeRequired": true,
    "podcastsBlocked": true,
    "proximityBlockSetupToNewDevice": true,
    "safariBlockAutofill": true,
    "safariBlockJavaScript": true,
    "safariBlockPopups": true,
    "safariBlocked": true,
    "safariCookieSettings": "blockAlways",
    "safariManagedDomains": [
      "Safari Managed Domains value"
    ],
    "safariPasswordAutoFillDomains": [
      "Safari Password Auto Fill Domains value"
    ],
    "safariRequireFraudWarning": true,
    "screenCaptureBlocked": true,
    "siriBlocked": true,
    "siriBlockedWhenLocked": true,
    "siriBlockUserGeneratedContent": true,
    "siriRequireProfanityFilter": true,
    "softwareUpdatesEnforcedDelayInDays": 2,
    "softwareUpdatesForceDelayed": true,
    "spotlightBlockInternetResults": true,
    "voiceDialingBlocked": true,
    "wallpaperBlockModification": true,
    "wiFiConnectOnlyToConfiguredNetworks": true,
    "classroomForceRequestPermissionToLeaveClasses": true,
    "keychainBlockCloudSync": true,
    "pkiBlockOTAUpdates": true,
    "privacyForceLimitAdTracking": true,
    "enterpriseBookBlockBackup": true,
    "enterpriseBookBlockMetadataSync": true,
    "airPrintBlocked": true,
    "airPrintBlockCredentialsStorage": true,
    "airPrintForceTrustedTLS": true,
    "airPrintBlockiBeaconDiscovery": true,
    "filesNetworkDriveAccessBlocked": true,
    "filesUsbDriveAccessBlocked": true,
    "wifiPowerOnForced": true,
    "blockSystemAppRemoval": true,
    "vpnBlockCreation": true,
    "appRemovalBlocked": true,
    "usbRestrictedModeBlocked": true,
    "passwordBlockAutoFill": true,
    "passwordBlockProximityRequests": true,
    "passwordBlockAirDropSharing": true,
    "dateAndTimeForceSetAutomatically": true,
    "contactsAllowManagedToUnmanagedWrite": true,
    "contactsAllowUnmanagedToManagedRead": true,
    "cellularBlockPersonalHotspotModification": true,
    "continuousPathKeyboardBlocked": true,
    "findMyDeviceInFindMyAppBlocked": true,
    "findMyFriendsInFindMyAppBlocked": true,
    "iTunesBlocked": true,
    "sharedDeviceBlockTemporarySessions": true,
    "kioskModeAppType": "appStoreApp"
  }
}
```



