---
title: 获取 iosManagedAppProtection
description: 读取 iosManagedAppProtection 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b31f8ab0927e164fd5c8d941c5ec281188cf54e3
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939800"
---
# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="7d34e-103">获取 iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="7d34e-103">Get iosManagedAppProtection</span></span>

> <span data-ttu-id="7d34e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7d34e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d34e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7d34e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d34e-106">读取 [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7d34e-106">Read properties and relationships of the [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d34e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7d34e-107">Prerequisites</span></span>
<span data-ttu-id="7d34e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7d34e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d34e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d34e-110">Permission type</span></span>|<span data-ttu-id="7d34e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7d34e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d34e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d34e-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7d34e-113">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="7d34e-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="7d34e-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d34e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="7d34e-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="7d34e-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="7d34e-116">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d34e-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7d34e-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d34e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d34e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d34e-118">Not supported.</span></span>|
|<span data-ttu-id="7d34e-119">Application</span><span class="sxs-lookup"><span data-stu-id="7d34e-119">Application</span></span>||
| <span data-ttu-id="7d34e-120">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="7d34e-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="7d34e-121">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d34e-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="7d34e-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="7d34e-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="7d34e-123">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d34e-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d34e-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d34e-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d34e-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7d34e-125">Optional query parameters</span></span>
<span data-ttu-id="7d34e-126">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7d34e-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d34e-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d34e-127">Request headers</span></span>
|<span data-ttu-id="7d34e-128">标头</span><span class="sxs-lookup"><span data-stu-id="7d34e-128">Header</span></span>|<span data-ttu-id="7d34e-129">值</span><span class="sxs-lookup"><span data-stu-id="7d34e-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d34e-130">授权</span><span class="sxs-lookup"><span data-stu-id="7d34e-130">Authorization</span></span>|<span data-ttu-id="7d34e-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7d34e-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d34e-132">接受</span><span class="sxs-lookup"><span data-stu-id="7d34e-132">Accept</span></span>|<span data-ttu-id="7d34e-133">application/json</span><span class="sxs-lookup"><span data-stu-id="7d34e-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d34e-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d34e-134">Request body</span></span>
<span data-ttu-id="7d34e-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7d34e-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d34e-136">响应</span><span class="sxs-lookup"><span data-stu-id="7d34e-136">Response</span></span>
<span data-ttu-id="7d34e-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7d34e-137">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d34e-138">示例</span><span class="sxs-lookup"><span data-stu-id="7d34e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d34e-139">请求</span><span class="sxs-lookup"><span data-stu-id="7d34e-139">Request</span></span>
<span data-ttu-id="7d34e-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7d34e-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="7d34e-141">响应</span><span class="sxs-lookup"><span data-stu-id="7d34e-141">Response</span></span>
<span data-ttu-id="7d34e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7d34e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2944

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
    "version": "Version value",
    "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
    "periodOnlineBeforeAccessCheck": "PT35.0018757S",
    "allowedInboundDataTransferSources": "managedApps",
    "allowedOutboundDataTransferDestinations": "managedApps",
    "organizationalCredentialsRequired": true,
    "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
    "dataBackupBlocked": true,
    "deviceComplianceRequired": true,
    "managedBrowserToOpenLinksRequired": true,
    "saveAsBlocked": true,
    "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
    "pinRequired": true,
    "maximumPinRetries": 1,
    "simplePinBlocked": true,
    "minimumPinLength": 0,
    "pinCharacterSet": "alphanumericAndSymbol",
    "periodBeforePinReset": "PT3M29.6631862S",
    "allowedDataStorageLocations": [
      "sharePoint"
    ],
    "contactSyncBlocked": true,
    "printBlocked": true,
    "fingerprintBlocked": true,
    "disableAppPinIfDevicePinIsSet": true,
    "minimumRequiredOsVersion": "Minimum Required Os Version value",
    "minimumWarningOsVersion": "Minimum Warning Os Version value",
    "minimumRequiredAppVersion": "Minimum Required App Version value",
    "minimumWarningAppVersion": "Minimum Warning App Version value",
    "minimumWipeOsVersion": "Minimum Wipe Os Version value",
    "minimumWipeAppVersion": "Minimum Wipe App Version value",
    "appActionIfDeviceComplianceRequired": "wipe",
    "appActionIfMaximumPinRetriesExceeded": "wipe",
    "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
    "allowedOutboundClipboardSharingExceptionLength": 14,
    "notificationRestriction": "blockOrganizationalData",
    "isAssigned": true,
    "targetedAppManagementLevels": "unmanaged",
    "appDataEncryptionType": "afterDeviceRestart",
    "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
    "deployedAppCount": 0,
    "faceIdBlocked": true,
    "exemptedAppProtocols": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
    "allowedIosDeviceModels": "Allowed Ios Device Models value",
    "appActionIfIosDeviceModelNotAllowed": "wipe",
    "filterOpenInToOnlyManagedApps": true,
    "disableProtectionOfManagedOutboundOpenInData": true,
    "protectInboundDataFromUnknownSources": true,
    "customBrowserProtocol": "Custom Browser Protocol value"
  }
}
```








