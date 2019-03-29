---
title: 获取 managedAppProtection
description: 读取 managedAppProtection 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b4cdd615f1201a8ae98961f9f3b1a919d2f05a7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977448"
---
# <a name="get-managedappprotection"></a><span data-ttu-id="d3016-103">获取 managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="d3016-103">Get managedAppProtection</span></span>

> <span data-ttu-id="d3016-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3016-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3016-105">读取 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d3016-105">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3016-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d3016-106">Prerequisites</span></span>
<span data-ttu-id="d3016-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3016-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3016-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3016-109">Permission type</span></span>|<span data-ttu-id="d3016-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d3016-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3016-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3016-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3016-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3016-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d3016-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3016-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3016-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3016-114">Not supported.</span></span>|
|<span data-ttu-id="d3016-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3016-115">Application</span></span>|<span data-ttu-id="d3016-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3016-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3016-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3016-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3016-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d3016-118">Optional query parameters</span></span>
<span data-ttu-id="d3016-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d3016-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3016-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3016-120">Request headers</span></span>
|<span data-ttu-id="d3016-121">标头</span><span class="sxs-lookup"><span data-stu-id="d3016-121">Header</span></span>|<span data-ttu-id="d3016-122">值</span><span class="sxs-lookup"><span data-stu-id="d3016-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3016-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3016-123">Authorization</span></span>|<span data-ttu-id="d3016-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d3016-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3016-125">接受</span><span class="sxs-lookup"><span data-stu-id="d3016-125">Accept</span></span>|<span data-ttu-id="d3016-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3016-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3016-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3016-127">Request body</span></span>
<span data-ttu-id="d3016-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d3016-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3016-129">响应</span><span class="sxs-lookup"><span data-stu-id="d3016-129">Response</span></span>
<span data-ttu-id="d3016-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d3016-130">If successful, this method returns a `200 OK` response code and [managedAppProtection](../resources/intune-mam-managedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3016-131">示例</span><span class="sxs-lookup"><span data-stu-id="d3016-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3016-132">请求</span><span class="sxs-lookup"><span data-stu-id="d3016-132">Request</span></span>
<span data-ttu-id="d3016-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d3016-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="d3016-134">响应</span><span class="sxs-lookup"><span data-stu-id="d3016-134">Response</span></span>
<span data-ttu-id="d3016-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d3016-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1631

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "a6c064ce-64ce-a6c0-ce64-c0a6ce64c0a6",
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
    "minimumWarningAppVersion": "Minimum Warning App Version value"
  }
}
```



