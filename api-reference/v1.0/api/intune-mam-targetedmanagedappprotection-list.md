---
title: 列出 targetedManagedAppProtections
description: 列出 targetedManagedAppProtection 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9df054ec62106207af18706128953d41407929df
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177637"
---
# <a name="list-targetedmanagedappprotections"></a><span data-ttu-id="ad050-103">列出 targetedManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="ad050-103">List targetedManagedAppProtections</span></span>

<span data-ttu-id="ad050-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad050-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad050-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ad050-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad050-106">列出 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ad050-106">List properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad050-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ad050-107">Prerequisites</span></span>
<span data-ttu-id="ad050-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad050-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad050-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad050-110">Permission type</span></span>|<span data-ttu-id="ad050-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ad050-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad050-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad050-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ad050-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad050-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ad050-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad050-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad050-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad050-115">Not supported.</span></span>|
|<span data-ttu-id="ad050-116">Application</span><span class="sxs-lookup"><span data-stu-id="ad050-116">Application</span></span>|<span data-ttu-id="ad050-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad050-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad050-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad050-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="ad050-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad050-119">Request headers</span></span>
|<span data-ttu-id="ad050-120">标头</span><span class="sxs-lookup"><span data-stu-id="ad050-120">Header</span></span>|<span data-ttu-id="ad050-121">值</span><span class="sxs-lookup"><span data-stu-id="ad050-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad050-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad050-122">Authorization</span></span>|<span data-ttu-id="ad050-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ad050-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad050-124">接受</span><span class="sxs-lookup"><span data-stu-id="ad050-124">Accept</span></span>|<span data-ttu-id="ad050-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad050-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad050-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad050-126">Request body</span></span>
<span data-ttu-id="ad050-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ad050-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad050-128">响应</span><span class="sxs-lookup"><span data-stu-id="ad050-128">Response</span></span>
<span data-ttu-id="ad050-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ad050-129">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad050-130">示例</span><span class="sxs-lookup"><span data-stu-id="ad050-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad050-131">请求</span><span class="sxs-lookup"><span data-stu-id="ad050-131">Request</span></span>
<span data-ttu-id="ad050-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ad050-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="ad050-133">响应</span><span class="sxs-lookup"><span data-stu-id="ad050-133">Response</span></span>
<span data-ttu-id="ad050-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ad050-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1792

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "b6b92266-2266-b6b9-6622-b9b66622b9b6",
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
      "isAssigned": true
    }
  ]
}
```



