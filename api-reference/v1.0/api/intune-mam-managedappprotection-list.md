---
title: 列出 managedAppProtections
description: 列出 managedAppProtection 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 41708d03b7bd7569237234e004987dd9caf5c381
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257139"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="cebfb-103">列出 managedAppProtections</span><span class="sxs-lookup"><span data-stu-id="cebfb-103">List managedAppProtections</span></span>

> <span data-ttu-id="cebfb-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cebfb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cebfb-105">列出 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cebfb-105">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cebfb-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="cebfb-106">Prerequisites</span></span>
<span data-ttu-id="cebfb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cebfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cebfb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cebfb-109">Permission type</span></span>|<span data-ttu-id="cebfb-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cebfb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cebfb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cebfb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cebfb-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cebfb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cebfb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cebfb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cebfb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cebfb-114">Not supported.</span></span>|
|<span data-ttu-id="cebfb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cebfb-115">Application</span></span>|<span data-ttu-id="cebfb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cebfb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cebfb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cebfb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="cebfb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cebfb-118">Request headers</span></span>
|<span data-ttu-id="cebfb-119">标头</span><span class="sxs-lookup"><span data-stu-id="cebfb-119">Header</span></span>|<span data-ttu-id="cebfb-120">值</span><span class="sxs-lookup"><span data-stu-id="cebfb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cebfb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cebfb-121">Authorization</span></span>|<span data-ttu-id="cebfb-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cebfb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cebfb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cebfb-123">Accept</span></span>|<span data-ttu-id="cebfb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cebfb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cebfb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cebfb-125">Request body</span></span>
<span data-ttu-id="cebfb-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cebfb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cebfb-127">响应</span><span class="sxs-lookup"><span data-stu-id="cebfb-127">Response</span></span>
<span data-ttu-id="cebfb-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cebfb-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cebfb-129">示例</span><span class="sxs-lookup"><span data-stu-id="cebfb-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="cebfb-130">请求</span><span class="sxs-lookup"><span data-stu-id="cebfb-130">Request</span></span>
<span data-ttu-id="cebfb-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cebfb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="cebfb-132">响应</span><span class="sxs-lookup"><span data-stu-id="cebfb-132">Response</span></span>
<span data-ttu-id="cebfb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cebfb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1715

{
  "value": [
    {
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
  ]
}
```



