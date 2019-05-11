---
title: 列出 androidDeviceOwnerGeneralDeviceConfigurations
description: 列出 androidDeviceOwnerGeneralDeviceConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7118b649e127aae016dc5fb9cb0c82a0dfa18902
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933198"
---
# <a name="list-androiddeviceownergeneraldeviceconfigurations"></a><span data-ttu-id="5a6bb-103">列出 androidDeviceOwnerGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="5a6bb-103">List androidDeviceOwnerGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="5a6bb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5a6bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a6bb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5a6bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a6bb-106">列出[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5a6bb-106">List properties and relationships of the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a6bb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5a6bb-107">Prerequisites</span></span>
<span data-ttu-id="5a6bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a6bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a6bb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a6bb-110">Permission type</span></span>|<span data-ttu-id="5a6bb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5a6bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a6bb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a6bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a6bb-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a6bb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5a6bb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a6bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a6bb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a6bb-115">Not supported.</span></span>|
|<span data-ttu-id="5a6bb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a6bb-116">Application</span></span>|<span data-ttu-id="5a6bb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a6bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a6bb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a6bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5a6bb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a6bb-119">Request headers</span></span>
|<span data-ttu-id="5a6bb-120">标头</span><span class="sxs-lookup"><span data-stu-id="5a6bb-120">Header</span></span>|<span data-ttu-id="5a6bb-121">值</span><span class="sxs-lookup"><span data-stu-id="5a6bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a6bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a6bb-122">Authorization</span></span>|<span data-ttu-id="5a6bb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5a6bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a6bb-124">接受</span><span class="sxs-lookup"><span data-stu-id="5a6bb-124">Accept</span></span>|<span data-ttu-id="5a6bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a6bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a6bb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a6bb-126">Request body</span></span>
<span data-ttu-id="5a6bb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5a6bb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a6bb-128">响应</span><span class="sxs-lookup"><span data-stu-id="5a6bb-128">Response</span></span>
<span data-ttu-id="5a6bb-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="5a6bb-129">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a6bb-130">示例</span><span class="sxs-lookup"><span data-stu-id="5a6bb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a6bb-131">请求</span><span class="sxs-lookup"><span data-stu-id="5a6bb-131">Request</span></span>
<span data-ttu-id="5a6bb-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5a6bb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="5a6bb-133">响应</span><span class="sxs-lookup"><span data-stu-id="5a6bb-133">Response</span></span>
<span data-ttu-id="5a6bb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5a6bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3438

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
      "dataRoamingBlocked": true,
      "dateTimeConfigurationBlocked": true,
      "factoryResetDeviceAdministratorEmails": [
        "Factory Reset Device Administrator Emails value"
      ],
      "factoryResetBlocked": true,
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
      "kioskModeBluetoothConfigurationEnabled": true,
      "kioskModeWiFiConfigurationEnabled": true,
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
      "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
      "vpnAlwaysOnLockdownMode": true,
      "wifiBlockEditConfigurations": true,
      "wifiBlockEditPolicyDefinedConfigurations": true
    }
  ]
}
```




