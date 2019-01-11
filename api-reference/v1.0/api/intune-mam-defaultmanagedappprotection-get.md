---
title: 获取 defaultManagedAppProtection
description: 读取 defaultManagedAppProtection 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c14fa93de18bfdb649ff049a89c797ae74beae7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833785"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="b5f48-103">获取 defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="b5f48-103">Get defaultManagedAppProtection</span></span>

> <span data-ttu-id="b5f48-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b5f48-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5f48-105">读取 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b5f48-105">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b5f48-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5f48-106">Prerequisites</span></span>
<span data-ttu-id="b5f48-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b5f48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5f48-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5f48-109">Permission type</span></span>|<span data-ttu-id="b5f48-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b5f48-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5f48-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5f48-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b5f48-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5f48-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b5f48-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5f48-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5f48-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5f48-114">Not supported.</span></span>|
|<span data-ttu-id="b5f48-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5f48-115">Application</span></span>|<span data-ttu-id="b5f48-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5f48-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5f48-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5f48-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5f48-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b5f48-118">Optional query parameters</span></span>
<span data-ttu-id="b5f48-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b5f48-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b5f48-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5f48-120">Request headers</span></span>
|<span data-ttu-id="b5f48-121">标头</span><span class="sxs-lookup"><span data-stu-id="b5f48-121">Header</span></span>|<span data-ttu-id="b5f48-122">值</span><span class="sxs-lookup"><span data-stu-id="b5f48-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5f48-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5f48-123">Authorization</span></span>|<span data-ttu-id="b5f48-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5f48-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5f48-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b5f48-125">Accept</span></span>|<span data-ttu-id="b5f48-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5f48-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5f48-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5f48-127">Request body</span></span>
<span data-ttu-id="b5f48-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5f48-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5f48-129">响应</span><span class="sxs-lookup"><span data-stu-id="b5f48-129">Response</span></span>
<span data-ttu-id="b5f48-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5f48-130">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5f48-131">示例</span><span class="sxs-lookup"><span data-stu-id="b5f48-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5f48-132">请求</span><span class="sxs-lookup"><span data-stu-id="b5f48-132">Request</span></span>
<span data-ttu-id="b5f48-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5f48-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="b5f48-134">响应</span><span class="sxs-lookup"><span data-stu-id="b5f48-134">Response</span></span>
<span data-ttu-id="b5f48-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5f48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2264

{
  "value": {
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
}
```



