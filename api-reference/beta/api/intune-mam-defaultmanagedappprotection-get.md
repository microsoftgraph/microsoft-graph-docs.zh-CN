---
title: 获取 defaultManagedAppProtection
description: 读取 defaultManagedAppProtection 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2d7e8cd56a295fe3e0bf1024168ec823bddd4dec
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145465"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="7a855-103">获取 defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="7a855-103">Get defaultManagedAppProtection</span></span>

<span data-ttu-id="7a855-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a855-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a855-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7a855-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a855-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a855-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a855-107">读取 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7a855-107">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a855-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7a855-108">Prerequisites</span></span>
<span data-ttu-id="7a855-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a855-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a855-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a855-111">Permission type</span></span>|<span data-ttu-id="7a855-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a855-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a855-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a855-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a855-114">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a855-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7a855-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a855-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a855-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a855-116">Not supported.</span></span>|
|<span data-ttu-id="7a855-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a855-117">Application</span></span>|<span data-ttu-id="7a855-118">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a855-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a855-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a855-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a855-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7a855-120">Optional query parameters</span></span>
<span data-ttu-id="7a855-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7a855-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a855-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a855-122">Request headers</span></span>
|<span data-ttu-id="7a855-123">标头</span><span class="sxs-lookup"><span data-stu-id="7a855-123">Header</span></span>|<span data-ttu-id="7a855-124">值</span><span class="sxs-lookup"><span data-stu-id="7a855-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a855-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a855-125">Authorization</span></span>|<span data-ttu-id="7a855-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7a855-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a855-127">接受</span><span class="sxs-lookup"><span data-stu-id="7a855-127">Accept</span></span>|<span data-ttu-id="7a855-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7a855-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a855-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a855-129">Request body</span></span>
<span data-ttu-id="7a855-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7a855-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a855-131">响应</span><span class="sxs-lookup"><span data-stu-id="7a855-131">Response</span></span>
<span data-ttu-id="7a855-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7a855-132">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a855-133">示例</span><span class="sxs-lookup"><span data-stu-id="7a855-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a855-134">请求</span><span class="sxs-lookup"><span data-stu-id="7a855-134">Request</span></span>
<span data-ttu-id="7a855-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7a855-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="7a855-136">响应</span><span class="sxs-lookup"><span data-stu-id="7a855-136">Response</span></span>
<span data-ttu-id="7a855-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7a855-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5743

{
  "value": {
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
    "maximumRequiredOsVersion": "Maximum Required Os Version value",
    "maximumWarningOsVersion": "Maximum Warning Os Version value",
    "maximumWipeOsVersion": "Maximum Wipe Os Version value",
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
    "appActionIfAndroidDeviceModelNotAllowed": "wipe",
    "customDialerAppProtocol": "Custom Dialer App Protocol value",
    "customDialerAppPackageId": "Custom Dialer App Package Id value",
    "customDialerAppDisplayName": "Custom Dialer App Display Name value",
    "biometricAuthenticationBlocked": true,
    "requiredAndroidSafetyNetEvaluationType": "hardwareBacked",
    "blockAfterCompanyPortalUpdateDeferralInDays": 11,
    "warnAfterCompanyPortalUpdateDeferralInDays": 10,
    "wipeAfterCompanyPortalUpdateDeferralInDays": 10,
    "deviceLockRequired": true,
    "appActionIfDeviceLockNotSet": "wipe"
  }
}
```




