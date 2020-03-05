---
title: 列出 defaultManagedAppProtections
description: 列出 defaultManagedAppProtection 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e7cd1fb49ae279e45015d5eabb46265f7f95b70a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463641"
---
# <a name="list-defaultmanagedappprotections"></a><span data-ttu-id="58e63-103">列出 defaultManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="58e63-103">List defaultManagedAppProtections</span></span>

<span data-ttu-id="58e63-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="58e63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58e63-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="58e63-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58e63-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58e63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58e63-107">列出 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="58e63-107">List properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58e63-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="58e63-108">Prerequisites</span></span>
<span data-ttu-id="58e63-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58e63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58e63-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="58e63-111">Permission type</span></span>|<span data-ttu-id="58e63-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="58e63-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58e63-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58e63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58e63-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="58e63-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="58e63-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58e63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58e63-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="58e63-116">Not supported.</span></span>|
|<span data-ttu-id="58e63-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="58e63-117">Application</span></span>|<span data-ttu-id="58e63-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="58e63-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58e63-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58e63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="58e63-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="58e63-120">Request headers</span></span>
|<span data-ttu-id="58e63-121">标头</span><span class="sxs-lookup"><span data-stu-id="58e63-121">Header</span></span>|<span data-ttu-id="58e63-122">值</span><span class="sxs-lookup"><span data-stu-id="58e63-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58e63-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58e63-123">Authorization</span></span>|<span data-ttu-id="58e63-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="58e63-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58e63-125">接受</span><span class="sxs-lookup"><span data-stu-id="58e63-125">Accept</span></span>|<span data-ttu-id="58e63-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58e63-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58e63-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="58e63-127">Request body</span></span>
<span data-ttu-id="58e63-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="58e63-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58e63-129">响应</span><span class="sxs-lookup"><span data-stu-id="58e63-129">Response</span></span>
<span data-ttu-id="58e63-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="58e63-130">If successful, this method returns a `200 OK` response code and a collection of [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58e63-131">示例</span><span class="sxs-lookup"><span data-stu-id="58e63-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="58e63-132">请求</span><span class="sxs-lookup"><span data-stu-id="58e63-132">Request</span></span>
<span data-ttu-id="58e63-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="58e63-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="58e63-134">响应</span><span class="sxs-lookup"><span data-stu-id="58e63-134">Response</span></span>
<span data-ttu-id="58e63-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="58e63-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5160

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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
      "exemptedAppProtocols": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "exemptedAppPackages": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "faceIdBlocked": true,
      "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
      "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
      "allowedIosDeviceModels": "Allowed Ios Device Models value",
      "appActionIfIosDeviceModelNotAllowed": "wipe",
      "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
      "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
      "thirdPartyKeyboardsBlocked": true,
      "filterOpenInToOnlyManagedApps": true,
      "disableProtectionOfManagedOutboundOpenInData": true,
      "protectInboundDataFromUnknownSources": true,
      "requiredAndroidSafetyNetDeviceAttestationType": "basicIntegrity",
      "appActionIfAndroidSafetyNetDeviceAttestationFailed": "wipe",
      "requiredAndroidSafetyNetAppsVerificationType": "enabled",
      "appActionIfAndroidSafetyNetAppsVerificationFailed": "wipe",
      "customBrowserProtocol": "Custom Browser Protocol value",
      "customBrowserPackageId": "Custom Browser Package Id value",
      "customBrowserDisplayName": "Custom Browser Display Name value",
      "minimumRequiredCompanyPortalVersion": "Minimum Required Company Portal Version value",
      "minimumWarningCompanyPortalVersion": "Minimum Warning Company Portal Version value",
      "minimumWipeCompanyPortalVersion": "Minimum Wipe Company Portal Version value",
      "allowedAndroidDeviceModels": [
        "Allowed Android Device Models value"
      ],
      "appActionIfAndroidDeviceModelNotAllowed": "wipe"
    }
  ]
}
```





