---
title: 列出 defaultManagedAppProtections
description: 列出 defaultManagedAppProtection 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7eb1c8fb0c82f66c8da357cad66a867fb3bfa3b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877642"
---
# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="9facb-103">列出 defaultManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="9facb-103">List defaultManagedAppProtections</span></span>

> <span data-ttu-id="9facb-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9facb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9facb-105">列出 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9facb-105">List properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9facb-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9facb-106">Prerequisites</span></span>
<span data-ttu-id="9facb-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9facb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9facb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9facb-109">Permission type</span></span>|<span data-ttu-id="9facb-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9facb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9facb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9facb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9facb-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9facb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9facb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9facb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9facb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9facb-114">Not supported.</span></span>|
|<span data-ttu-id="9facb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9facb-115">Application</span></span>|<span data-ttu-id="9facb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9facb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9facb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9facb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="9facb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9facb-118">Request headers</span></span>
|<span data-ttu-id="9facb-119">标头</span><span class="sxs-lookup"><span data-stu-id="9facb-119">Header</span></span>|<span data-ttu-id="9facb-120">值</span><span class="sxs-lookup"><span data-stu-id="9facb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9facb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9facb-121">Authorization</span></span>|<span data-ttu-id="9facb-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9facb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9facb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9facb-123">Accept</span></span>|<span data-ttu-id="9facb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9facb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9facb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9facb-125">Request body</span></span>
<span data-ttu-id="9facb-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9facb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9facb-127">响应</span><span class="sxs-lookup"><span data-stu-id="9facb-127">Response</span></span>
<span data-ttu-id="9facb-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9facb-128">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9facb-129">示例</span><span class="sxs-lookup"><span data-stu-id="9facb-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9facb-130">请求</span><span class="sxs-lookup"><span data-stu-id="9facb-130">Request</span></span>
<span data-ttu-id="9facb-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9facb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="9facb-132">响应</span><span class="sxs-lookup"><span data-stu-id="9facb-132">Response</span></span>
<span data-ttu-id="9facb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9facb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2380

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "77064c51-4c51-7706-514c-0677514c0677",
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
      "appDataEncryptionType": "afterDeviceRestart",
      "screenCaptureBlocked": true,
      "encryptAppData": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
      "faceIdBlocked": true
    }
  ]
}
```



