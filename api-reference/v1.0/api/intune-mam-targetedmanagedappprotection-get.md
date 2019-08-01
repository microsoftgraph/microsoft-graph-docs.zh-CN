---
title: 获取 targetedManagedAppProtection
description: 读取 targetedManagedAppProtection 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ffeb24371241ede90f12b1b9618e3e96e766ed73
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018103"
---
# <a name="get-targetedmanagedappprotection"></a><span data-ttu-id="c0e09-103">获取 targetedManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="c0e09-103">Get targetedManagedAppProtection</span></span>

> <span data-ttu-id="c0e09-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0e09-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0e09-105">读取 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c0e09-105">Read properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0e09-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="c0e09-106">Prerequisites</span></span>
<span data-ttu-id="c0e09-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0e09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0e09-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0e09-109">Permission type</span></span>|<span data-ttu-id="c0e09-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c0e09-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0e09-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0e09-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c0e09-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0e09-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c0e09-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0e09-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0e09-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0e09-114">Not supported.</span></span>|
|<span data-ttu-id="c0e09-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0e09-115">Application</span></span>|<span data-ttu-id="c0e09-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0e09-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0e09-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0e09-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0e09-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c0e09-118">Optional query parameters</span></span>
<span data-ttu-id="c0e09-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c0e09-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0e09-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0e09-120">Request headers</span></span>
|<span data-ttu-id="c0e09-121">标头</span><span class="sxs-lookup"><span data-stu-id="c0e09-121">Header</span></span>|<span data-ttu-id="c0e09-122">值</span><span class="sxs-lookup"><span data-stu-id="c0e09-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0e09-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0e09-123">Authorization</span></span>|<span data-ttu-id="c0e09-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c0e09-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0e09-125">接受</span><span class="sxs-lookup"><span data-stu-id="c0e09-125">Accept</span></span>|<span data-ttu-id="c0e09-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0e09-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0e09-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0e09-127">Request body</span></span>
<span data-ttu-id="c0e09-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0e09-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0e09-129">响应</span><span class="sxs-lookup"><span data-stu-id="c0e09-129">Response</span></span>
<span data-ttu-id="c0e09-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0e09-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0e09-131">示例</span><span class="sxs-lookup"><span data-stu-id="c0e09-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0e09-132">请求</span><span class="sxs-lookup"><span data-stu-id="c0e09-132">Request</span></span>
<span data-ttu-id="c0e09-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0e09-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="c0e09-134">响应</span><span class="sxs-lookup"><span data-stu-id="c0e09-134">Response</span></span>
<span data-ttu-id="c0e09-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c0e09-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1664

{
  "value": {
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
    "isAssigned": true
  }
}
```



