---
title: 列出 iosManagedAppProtections
description: 列出 iosManagedAppProtection 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 8a44dd40d15deb99febe4d13ca1badad128106ef
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329755"
---
# <a name="list-iosmanagedappprotections"></a><span data-ttu-id="4c3c0-103">列出 iosManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="4c3c0-103">List iosManagedAppProtections</span></span>

> <span data-ttu-id="4c3c0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4c3c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c3c0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4c3c0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c3c0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4c3c0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c3c0-107">列出 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4c3c0-107">List properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c3c0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4c3c0-108">Prerequisites</span></span>
<span data-ttu-id="4c3c0-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="4c3c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c3c0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c3c0-111">Permission type</span></span>|<span data-ttu-id="4c3c0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4c3c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c3c0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c3c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c3c0-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c3c0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4c3c0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c3c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c3c0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c3c0-116">Not supported.</span></span>|
|<span data-ttu-id="4c3c0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c3c0-117">Application</span></span>|<span data-ttu-id="4c3c0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c3c0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c3c0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c3c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="4c3c0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c3c0-120">Request headers</span></span>
|<span data-ttu-id="4c3c0-121">标头</span><span class="sxs-lookup"><span data-stu-id="4c3c0-121">Header</span></span>|<span data-ttu-id="4c3c0-122">值</span><span class="sxs-lookup"><span data-stu-id="4c3c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c3c0-123">授权</span><span class="sxs-lookup"><span data-stu-id="4c3c0-123">Authorization</span></span>|<span data-ttu-id="4c3c0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4c3c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c3c0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4c3c0-125">Accept</span></span>|<span data-ttu-id="4c3c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c3c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c3c0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c3c0-127">Request body</span></span>
<span data-ttu-id="4c3c0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4c3c0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c3c0-129">响应</span><span class="sxs-lookup"><span data-stu-id="4c3c0-129">Response</span></span>
<span data-ttu-id="4c3c0-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4c3c0-130">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c3c0-131">示例</span><span class="sxs-lookup"><span data-stu-id="4c3c0-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c3c0-132">请求</span><span class="sxs-lookup"><span data-stu-id="4c3c0-132">Request</span></span>
<span data-ttu-id="4c3c0-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4c3c0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="4c3c0-134">响应</span><span class="sxs-lookup"><span data-stu-id="4c3c0-134">Response</span></span>
<span data-ttu-id="4c3c0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4c3c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2870

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
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
      "isAssigned": true,
      "targetedAppManagementLevels": "unmanaged",
      "appDataEncryptionType": "afterDeviceRestart",
      "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
      "deployedAppCount": 0,
      "faceIdBlocked": true,
      "exemptedAppProtocols": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
      "allowedIosDeviceModels": "Allowed Ios Device Models value",
      "appActionIfIosDeviceModelNotAllowed": "wipe",
      "thirdPartyKeyboardsBlocked": true,
      "filterOpenInToOnlyManagedApps": true,
      "disableProtectionOfManagedOutboundOpenInData": true,
      "protectInboundDataFromUnknownSources": true
    }
  ]
}
```





