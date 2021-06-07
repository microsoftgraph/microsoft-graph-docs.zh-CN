---
title: 列出 defaultManagedAppProtections
description: 列出 defaultManagedAppProtection 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bf7a1f8bef68cee9b57614d43c02aa957515b5e7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758120"
---
# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="6a837-103">列出 defaultManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="6a837-103">List defaultManagedAppProtections</span></span>

<span data-ttu-id="6a837-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a837-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a837-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a837-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a837-106">列出 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6a837-106">List properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a837-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6a837-107">Prerequisites</span></span>
<span data-ttu-id="6a837-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a837-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a837-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a837-110">Permission type</span></span>|<span data-ttu-id="6a837-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a837-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a837-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a837-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a837-113">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a837-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6a837-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a837-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a837-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a837-115">Not supported.</span></span>|
|<span data-ttu-id="6a837-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a837-116">Application</span></span>|<span data-ttu-id="6a837-117">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a837-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a837-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a837-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="6a837-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a837-119">Request headers</span></span>
|<span data-ttu-id="6a837-120">标头</span><span class="sxs-lookup"><span data-stu-id="6a837-120">Header</span></span>|<span data-ttu-id="6a837-121">值</span><span class="sxs-lookup"><span data-stu-id="6a837-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a837-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a837-122">Authorization</span></span>|<span data-ttu-id="6a837-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6a837-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a837-124">接受</span><span class="sxs-lookup"><span data-stu-id="6a837-124">Accept</span></span>|<span data-ttu-id="6a837-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a837-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a837-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a837-126">Request body</span></span>
<span data-ttu-id="6a837-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6a837-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a837-128">响应</span><span class="sxs-lookup"><span data-stu-id="6a837-128">Response</span></span>
<span data-ttu-id="6a837-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6a837-129">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a837-130">示例</span><span class="sxs-lookup"><span data-stu-id="6a837-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a837-131">请求</span><span class="sxs-lookup"><span data-stu-id="6a837-131">Request</span></span>
<span data-ttu-id="6a837-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a837-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="6a837-133">响应</span><span class="sxs-lookup"><span data-stu-id="6a837-133">Response</span></span>
<span data-ttu-id="6a837-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a837-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2422

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
      "managedBrowser": "microsoftEdge",
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




