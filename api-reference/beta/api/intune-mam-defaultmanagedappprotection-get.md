---
title: 获取 defaultManagedAppProtection
description: 读取 defaultManagedAppProtection 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c6745545ce71dc486207efaa2ff95511418750b1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919482"
---
# <a name="get-defaultmanagedappprotection"></a><span data-ttu-id="a9d2e-103">获取 defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="a9d2e-103">Get defaultManagedAppProtection</span></span>

> <span data-ttu-id="a9d2e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a9d2e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9d2e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a9d2e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9d2e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a9d2e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9d2e-107">读取 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a9d2e-107">Read properties and relationships of the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9d2e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a9d2e-108">Prerequisites</span></span>
<span data-ttu-id="a9d2e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a9d2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9d2e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9d2e-111">Permission type</span></span>|<span data-ttu-id="a9d2e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a9d2e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9d2e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9d2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9d2e-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9d2e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a9d2e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9d2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9d2e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9d2e-116">Not supported.</span></span>|
|<span data-ttu-id="a9d2e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9d2e-117">Application</span></span>|<span data-ttu-id="a9d2e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9d2e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9d2e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9d2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9d2e-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a9d2e-120">Optional query parameters</span></span>
<span data-ttu-id="a9d2e-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a9d2e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a9d2e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9d2e-122">Request headers</span></span>
|<span data-ttu-id="a9d2e-123">标头</span><span class="sxs-lookup"><span data-stu-id="a9d2e-123">Header</span></span>|<span data-ttu-id="a9d2e-124">值</span><span class="sxs-lookup"><span data-stu-id="a9d2e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9d2e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9d2e-125">Authorization</span></span>|<span data-ttu-id="a9d2e-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a9d2e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9d2e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a9d2e-127">Accept</span></span>|<span data-ttu-id="a9d2e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a9d2e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9d2e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9d2e-129">Request body</span></span>
<span data-ttu-id="a9d2e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a9d2e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9d2e-131">响应</span><span class="sxs-lookup"><span data-stu-id="a9d2e-131">Response</span></span>
<span data-ttu-id="a9d2e-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9d2e-132">If successful, this method returns a `200 OK` response code and [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9d2e-133">示例</span><span class="sxs-lookup"><span data-stu-id="a9d2e-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9d2e-134">请求</span><span class="sxs-lookup"><span data-stu-id="a9d2e-134">Request</span></span>
<span data-ttu-id="a9d2e-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9d2e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="a9d2e-136">响应</span><span class="sxs-lookup"><span data-stu-id="a9d2e-136">Response</span></span>
<span data-ttu-id="a9d2e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a9d2e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3506

{
  "value": {
    "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
    "protectInboundDataFromUnknownSources": true
  }
}
```





