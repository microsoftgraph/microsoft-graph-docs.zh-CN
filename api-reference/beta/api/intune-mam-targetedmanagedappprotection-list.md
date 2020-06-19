---
title: 列出 targetedManagedAppProtections
description: 列出 targetedManagedAppProtection 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c4e73fad4f577accd9bdfe8b86d0280f51d6f37
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791880"
---
# <a name="list-targetedmanagedappprotections"></a><span data-ttu-id="514e3-103">列出 targetedManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="514e3-103">List targetedManagedAppProtections</span></span>

<span data-ttu-id="514e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="514e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="514e3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="514e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="514e3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="514e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="514e3-107">列出 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="514e3-107">List properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="514e3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="514e3-108">Prerequisites</span></span>
<span data-ttu-id="514e3-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="514e3-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="514e3-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="514e3-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="514e3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="514e3-111">Permission type</span></span>|<span data-ttu-id="514e3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="514e3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="514e3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="514e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="514e3-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="514e3-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="514e3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="514e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="514e3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="514e3-116">Not supported.</span></span>|
|<span data-ttu-id="514e3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="514e3-117">Application</span></span>|<span data-ttu-id="514e3-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="514e3-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="514e3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="514e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="514e3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="514e3-120">Request headers</span></span>
|<span data-ttu-id="514e3-121">标头</span><span class="sxs-lookup"><span data-stu-id="514e3-121">Header</span></span>|<span data-ttu-id="514e3-122">值</span><span class="sxs-lookup"><span data-stu-id="514e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="514e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="514e3-123">Authorization</span></span>|<span data-ttu-id="514e3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="514e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="514e3-125">接受</span><span class="sxs-lookup"><span data-stu-id="514e3-125">Accept</span></span>|<span data-ttu-id="514e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="514e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="514e3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="514e3-127">Request body</span></span>
<span data-ttu-id="514e3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="514e3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="514e3-129">响应</span><span class="sxs-lookup"><span data-stu-id="514e3-129">Response</span></span>
<span data-ttu-id="514e3-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="514e3-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="514e3-131">示例</span><span class="sxs-lookup"><span data-stu-id="514e3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="514e3-132">请求</span><span class="sxs-lookup"><span data-stu-id="514e3-132">Request</span></span>
<span data-ttu-id="514e3-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="514e3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="514e3-134">响应</span><span class="sxs-lookup"><span data-stu-id="514e3-134">Response</span></span>
<span data-ttu-id="514e3-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="514e3-135">Here is an example of the response.</span></span> <span data-ttu-id="514e3-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="514e3-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="514e3-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="514e3-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2723

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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
      "minimumWipeOsVersion": "Minimum Wipe Os Version value",
      "minimumWipeAppVersion": "Minimum Wipe App Version value",
      "appActionIfDeviceComplianceRequired": "wipe",
      "appActionIfMaximumPinRetriesExceeded": "wipe",
      "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
      "allowedOutboundClipboardSharingExceptionLength": 14,
      "notificationRestriction": "blockOrganizationalData",
      "previousPinBlockCount": 5,
      "managedBrowser": "microsoftEdge",
      "maximumAllowedDeviceThreatLevel": "secured",
      "mobileThreatDefenseRemediationAction": "wipe",
      "blockDataIngestionIntoOrganizationDocuments": true,
      "allowedDataIngestionLocations": [
        "sharePoint"
      ],
      "appActionIfUnableToAuthenticateUser": "wipe",
      "dialerRestrictionLevel": "managedApps",
      "isAssigned": true,
      "targetedAppManagementLevels": "unmanaged"
    }
  ]
}
```



