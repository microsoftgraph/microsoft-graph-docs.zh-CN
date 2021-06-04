---
title: 列出 managedAppProtections
description: 列出 managedAppProtection 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9ff9173889078fe89fc2966906d391e65bbf2dc9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753517"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="cf529-103">列出 managedAppProtections</span><span class="sxs-lookup"><span data-stu-id="cf529-103">List managedAppProtections</span></span>

<span data-ttu-id="cf529-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf529-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf529-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cf529-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf529-106">列出 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cf529-106">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf529-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cf529-107">Prerequisites</span></span>
<span data-ttu-id="cf529-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf529-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf529-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf529-110">Permission type</span></span>|<span data-ttu-id="cf529-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf529-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf529-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf529-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf529-113">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf529-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cf529-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf529-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf529-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf529-115">Not supported.</span></span>|
|<span data-ttu-id="cf529-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf529-116">Application</span></span>|<span data-ttu-id="cf529-117">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf529-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf529-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf529-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="cf529-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf529-119">Request headers</span></span>
|<span data-ttu-id="cf529-120">标头</span><span class="sxs-lookup"><span data-stu-id="cf529-120">Header</span></span>|<span data-ttu-id="cf529-121">值</span><span class="sxs-lookup"><span data-stu-id="cf529-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf529-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf529-122">Authorization</span></span>|<span data-ttu-id="cf529-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cf529-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf529-124">接受</span><span class="sxs-lookup"><span data-stu-id="cf529-124">Accept</span></span>|<span data-ttu-id="cf529-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cf529-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf529-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf529-126">Request body</span></span>
<span data-ttu-id="cf529-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf529-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf529-128">响应</span><span class="sxs-lookup"><span data-stu-id="cf529-128">Response</span></span>
<span data-ttu-id="cf529-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cf529-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf529-130">示例</span><span class="sxs-lookup"><span data-stu-id="cf529-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf529-131">请求</span><span class="sxs-lookup"><span data-stu-id="cf529-131">Request</span></span>
<span data-ttu-id="cf529-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf529-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="cf529-133">响应</span><span class="sxs-lookup"><span data-stu-id="cf529-133">Response</span></span>
<span data-ttu-id="cf529-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cf529-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1757

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
      "minimumWarningAppVersion": "Minimum Warning App Version value",
      "managedBrowser": "microsoftEdge"
    }
  ]
}
```




