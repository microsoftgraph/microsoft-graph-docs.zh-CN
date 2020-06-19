---
title: 列出 androidDeviceOwnerGeneralDeviceConfigurations
description: 列出 androidDeviceOwnerGeneralDeviceConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 50a9d91cae7975d259720219932872b4579ee183
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793120"
---
# <a name="list-androiddeviceownergeneraldeviceconfigurations"></a><span data-ttu-id="1ffc5-103">列出 androidDeviceOwnerGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="1ffc5-103">List androidDeviceOwnerGeneralDeviceConfigurations</span></span>

<span data-ttu-id="1ffc5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ffc5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ffc5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1ffc5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ffc5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ffc5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ffc5-107">列出[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1ffc5-107">List properties and relationships of the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ffc5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1ffc5-108">Prerequisites</span></span>
<span data-ttu-id="1ffc5-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1ffc5-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1ffc5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ffc5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ffc5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ffc5-111">Permission type</span></span>|<span data-ttu-id="1ffc5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1ffc5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ffc5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ffc5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ffc5-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ffc5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1ffc5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ffc5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ffc5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ffc5-116">Not supported.</span></span>|
|<span data-ttu-id="1ffc5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ffc5-117">Application</span></span>|<span data-ttu-id="1ffc5-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ffc5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ffc5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ffc5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1ffc5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ffc5-120">Request headers</span></span>
|<span data-ttu-id="1ffc5-121">标头</span><span class="sxs-lookup"><span data-stu-id="1ffc5-121">Header</span></span>|<span data-ttu-id="1ffc5-122">值</span><span class="sxs-lookup"><span data-stu-id="1ffc5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ffc5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ffc5-123">Authorization</span></span>|<span data-ttu-id="1ffc5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1ffc5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ffc5-125">接受</span><span class="sxs-lookup"><span data-stu-id="1ffc5-125">Accept</span></span>|<span data-ttu-id="1ffc5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ffc5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ffc5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ffc5-127">Request body</span></span>
<span data-ttu-id="1ffc5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ffc5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ffc5-129">响应</span><span class="sxs-lookup"><span data-stu-id="1ffc5-129">Response</span></span>
<span data-ttu-id="1ffc5-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="1ffc5-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ffc5-131">示例</span><span class="sxs-lookup"><span data-stu-id="1ffc5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ffc5-132">请求</span><span class="sxs-lookup"><span data-stu-id="1ffc5-132">Request</span></span>
<span data-ttu-id="1ffc5-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ffc5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1ffc5-134">响应</span><span class="sxs-lookup"><span data-stu-id="1ffc5-134">Response</span></span>
<span data-ttu-id="1ffc5-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1ffc5-135">Here is an example of the response.</span></span> <span data-ttu-id="1ffc5-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1ffc5-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1ffc5-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1ffc5-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5761

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
      "id": "edad943d-943d-edad-3d94-aded3d94aded",
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
      "accountsBlockModification": true,
      "appsAllowInstallFromUnknownSources": true,
      "appsAutoUpdatePolicy": "userChoice",
      "appsDefaultPermissionPolicy": "prompt",
      "appsRecommendSkippingFirstUseHints": true,
      "bluetoothBlockConfiguration": true,
      "bluetoothBlockContactSharing": true,
      "cameraBlocked": true,
      "cellularBlockWiFiTethering": true,
      "certificateCredentialConfigurationDisabled": true,
      "microsoftLauncherConfigurationEnabled": true,
      "microsoftLauncherCustomWallpaperEnabled": true,
      "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
      "microsoftLauncherCustomWallpaperAllowUserModification": true,
      "microsoftLauncherFeedEnabled": true,
      "microsoftLauncherFeedAllowUserModification": true,
      "microsoftLauncherDockPresenceConfiguration": "show",
      "microsoftLauncherDockPresenceAllowUserModification": true,
      "microsoftLauncherSearchBarPlacementConfiguration": "top",
      "microsoftLauncherSearchBarPlacementAllowUserModification": true,
      "enrollmentProfile": "dedicatedDevice",
      "dataRoamingBlocked": true,
      "dateTimeConfigurationBlocked": true,
      "factoryResetDeviceAdministratorEmails": [
        "Factory Reset Device Administrator Emails value"
      ],
      "factoryResetBlocked": true,
      "globalProxy": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
        "proxyAutoConfigURL": "Proxy Auto Config URL value"
      },
      "googleAccountsBlocked": true,
      "kioskModeScreenSaverConfigurationEnabled": true,
      "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
      "kioskModeScreenSaverDisplayTimeInSeconds": 8,
      "kioskModeScreenSaverStartDelayInSeconds": 7,
      "kioskModeScreenSaverDetectMediaDisabled": true,
      "kioskModeApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
      "kioskModeExitCode": "Kiosk Mode Exit Code value",
      "kioskModeVirtualHomeButtonEnabled": true,
      "kioskModeVirtualHomeButtonType": "swipeUp",
      "kioskModeBluetoothConfigurationEnabled": true,
      "kioskModeWiFiConfigurationEnabled": true,
      "kioskModeFlashlightConfigurationEnabled": true,
      "kioskModeMediaVolumeConfigurationEnabled": true,
      "microphoneForceMute": true,
      "networkEscapeHatchAllowed": true,
      "nfcBlockOutgoingBeam": true,
      "passwordBlockKeyguard": true,
      "passwordBlockKeyguardFeatures": [
        "camera"
      ],
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinimumLetterCharacters": 15,
      "passwordMinimumLowerCaseCharacters": 2,
      "passwordMinimumNonLetterCharacters": 2,
      "passwordMinimumNumericCharacters": 0,
      "passwordMinimumSymbolCharacters": 15,
      "passwordMinimumUpperCaseCharacters": 2,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordCountToBlock": 4,
      "passwordRequiredType": "required",
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "playStoreMode": "allowList",
      "safeBootBlocked": true,
      "screenCaptureBlocked": true,
      "securityAllowDebuggingFeatures": true,
      "securityRequireVerifyApps": true,
      "statusBarBlocked": true,
      "stayOnModes": [
        "ac"
      ],
      "storageAllowUsb": true,
      "storageBlockExternalMedia": true,
      "storageBlockUsbFileTransfer": true,
      "systemUpdateWindowStartMinutesAfterMidnight": 11,
      "systemUpdateWindowEndMinutesAfterMidnight": 9,
      "systemUpdateInstallType": "postpone",
      "systemWindowsBlocked": true,
      "usersBlockAdd": true,
      "usersBlockRemove": true,
      "volumeBlockAdjustment": true,
      "vpnAlwaysOnLockdownMode": true,
      "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
      "wifiBlockEditConfigurations": true,
      "wifiBlockEditPolicyDefinedConfigurations": true
    }
  ]
}
```



