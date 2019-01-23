---
title: 获取 androidDeviceOwnerGeneralDeviceConfiguration
description: 读取属性和 androidDeviceOwnerGeneralDeviceConfiguration 对象的关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 77714d5d4874e6ed2a974ea30ad5b6045f122e82
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405301"
---
# <a name="get-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="46663-103">获取 androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="46663-103">Get androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="46663-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="46663-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="46663-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="46663-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46663-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="46663-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46663-107">读取属性和[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="46663-107">Read properties and relationships of the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46663-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="46663-108">Prerequisites</span></span>
<span data-ttu-id="46663-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="46663-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="46663-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="46663-111">Permission type</span></span>|<span data-ttu-id="46663-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="46663-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46663-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46663-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46663-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="46663-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="46663-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46663-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46663-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="46663-116">Not supported.</span></span>|
|<span data-ttu-id="46663-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="46663-117">Application</span></span>|<span data-ttu-id="46663-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="46663-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46663-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46663-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46663-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="46663-120">Optional query parameters</span></span>
<span data-ttu-id="46663-121">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="46663-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46663-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="46663-122">Request headers</span></span>
|<span data-ttu-id="46663-123">标头</span><span class="sxs-lookup"><span data-stu-id="46663-123">Header</span></span>|<span data-ttu-id="46663-124">值</span><span class="sxs-lookup"><span data-stu-id="46663-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46663-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="46663-125">Authorization</span></span>|<span data-ttu-id="46663-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="46663-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46663-127">Accept</span><span class="sxs-lookup"><span data-stu-id="46663-127">Accept</span></span>|<span data-ttu-id="46663-128">application/json</span><span class="sxs-lookup"><span data-stu-id="46663-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46663-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="46663-129">Request body</span></span>
<span data-ttu-id="46663-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="46663-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46663-131">响应</span><span class="sxs-lookup"><span data-stu-id="46663-131">Response</span></span>
<span data-ttu-id="46663-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="46663-132">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46663-133">示例</span><span class="sxs-lookup"><span data-stu-id="46663-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="46663-134">请求</span><span class="sxs-lookup"><span data-stu-id="46663-134">Request</span></span>
<span data-ttu-id="46663-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46663-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="46663-136">响应</span><span class="sxs-lookup"><span data-stu-id="46663-136">Response</span></span>
<span data-ttu-id="46663-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="46663-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2854

{
  "value": {
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
    "microphoneForceMute": true,
    "networkEscapeHatchAllowed": true,
    "nfcBlockOutgoingBeam": true,
    "passwordBlockKeyguard": true,
    "passwordBlockKeyguardFeatures": [
      "camera"
    ],
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordCountToBlock": 4,
    "passwordRequiredType": "required",
    "passwordSignInFailureCountBeforeFactoryReset": 12,
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
}
```




