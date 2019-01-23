---
title: 列出 managedAppProtections
description: 列出 managedAppProtection 对象的属性和关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ed611086d0bdc52e0247104863238c025a1974b0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403922"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="0846b-103">列出 managedAppProtections</span><span class="sxs-lookup"><span data-stu-id="0846b-103">List managedAppProtections</span></span>

> <span data-ttu-id="0846b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0846b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0846b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0846b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0846b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0846b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0846b-107">列出 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0846b-107">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0846b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0846b-108">Prerequisites</span></span>
<span data-ttu-id="0846b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0846b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0846b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0846b-111">Permission type</span></span>|<span data-ttu-id="0846b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0846b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0846b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0846b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0846b-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0846b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0846b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0846b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0846b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0846b-116">Not supported.</span></span>|
|<span data-ttu-id="0846b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0846b-117">Application</span></span>|<span data-ttu-id="0846b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0846b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0846b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0846b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="0846b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0846b-120">Request headers</span></span>
|<span data-ttu-id="0846b-121">标头</span><span class="sxs-lookup"><span data-stu-id="0846b-121">Header</span></span>|<span data-ttu-id="0846b-122">值</span><span class="sxs-lookup"><span data-stu-id="0846b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0846b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0846b-123">Authorization</span></span>|<span data-ttu-id="0846b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0846b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0846b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0846b-125">Accept</span></span>|<span data-ttu-id="0846b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0846b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0846b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0846b-127">Request body</span></span>
<span data-ttu-id="0846b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0846b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0846b-129">响应</span><span class="sxs-lookup"><span data-stu-id="0846b-129">Response</span></span>
<span data-ttu-id="0846b-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedAppProtection](../resources/intune-mam-managedappprotection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0846b-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0846b-131">示例</span><span class="sxs-lookup"><span data-stu-id="0846b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0846b-132">请求</span><span class="sxs-lookup"><span data-stu-id="0846b-132">Request</span></span>
<span data-ttu-id="0846b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0846b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="0846b-134">响应</span><span class="sxs-lookup"><span data-stu-id="0846b-134">Response</span></span>
<span data-ttu-id="0846b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0846b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2094

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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
      "minimumWipeOsVersion": "Minimum Wipe Os Version value",
      "minimumWipeAppVersion": "Minimum Wipe App Version value",
      "appActionIfDeviceComplianceRequired": "wipe",
      "appActionIfMaximumPinRetriesExceeded": "wipe",
      "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S"
    }
  ]
}
```




