---
title: 列出 androidManagedAppProtections
description: 列出 androidManagedAppProtection 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ae8fcf08efe266dc34947fb6e7ad6b8c8fb2a36a
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864646"
---
# <a name="list-androidmanagedappprotections"></a><span data-ttu-id="f4aff-103">列出 androidManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="f4aff-103">List androidManagedAppProtections</span></span>

<span data-ttu-id="f4aff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4aff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4aff-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4aff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4aff-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4aff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4aff-107">列出 [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4aff-107">List properties and relationships of the [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4aff-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4aff-108">Prerequisites</span></span>
<span data-ttu-id="f4aff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4aff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4aff-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4aff-111">Permission type</span></span>|<span data-ttu-id="f4aff-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4aff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4aff-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4aff-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f4aff-114">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="f4aff-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="f4aff-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4aff-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="f4aff-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="f4aff-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f4aff-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4aff-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f4aff-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4aff-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4aff-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4aff-119">Not supported.</span></span>|
|<span data-ttu-id="f4aff-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4aff-120">Application</span></span>||
| <span data-ttu-id="f4aff-121">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="f4aff-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="f4aff-122">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4aff-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="f4aff-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="f4aff-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f4aff-124">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4aff-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4aff-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4aff-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="f4aff-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4aff-126">Request headers</span></span>
|<span data-ttu-id="f4aff-127">标头</span><span class="sxs-lookup"><span data-stu-id="f4aff-127">Header</span></span>|<span data-ttu-id="f4aff-128">值</span><span class="sxs-lookup"><span data-stu-id="f4aff-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4aff-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4aff-129">Authorization</span></span>|<span data-ttu-id="f4aff-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4aff-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4aff-131">接受</span><span class="sxs-lookup"><span data-stu-id="f4aff-131">Accept</span></span>|<span data-ttu-id="f4aff-132">application/json</span><span class="sxs-lookup"><span data-stu-id="f4aff-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4aff-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4aff-133">Request body</span></span>
<span data-ttu-id="f4aff-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4aff-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4aff-135">响应</span><span class="sxs-lookup"><span data-stu-id="f4aff-135">Response</span></span>
<span data-ttu-id="f4aff-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f4aff-136">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4aff-137">示例</span><span class="sxs-lookup"><span data-stu-id="f4aff-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4aff-138">请求</span><span class="sxs-lookup"><span data-stu-id="f4aff-138">Request</span></span>
<span data-ttu-id="f4aff-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4aff-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="f4aff-140">响应</span><span class="sxs-lookup"><span data-stu-id="f4aff-140">Response</span></span>
<span data-ttu-id="f4aff-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4aff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3448

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
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
      "isAssigned": true,
      "targetedAppManagementLevels": "unmanaged",
      "screenCaptureBlocked": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "encryptAppData": true,
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
      "exemptedAppPackages": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
      "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
      "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
      "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
      "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
      "requiredAndroidSafetyNetAppsVerificationType": "enabled",
      "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe",
      "customBrowserPackageId": "Custom Browser Package Id value",
      "customBrowserDisplayName": "Custom Browser Display Name value"
    }
  ]
}
```







