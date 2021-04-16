---
title: 获取 iosManagedAppProtection
description: 读取 iosManagedAppProtection 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9159bf09d9b97f78582a9c1efb9fecef2ad071e9
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863105"
---
# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="88d7e-103">获取 iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="88d7e-103">Get iosManagedAppProtection</span></span>

<span data-ttu-id="88d7e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88d7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88d7e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="88d7e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88d7e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88d7e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88d7e-107">读取 [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88d7e-107">Read properties and relationships of the [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88d7e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="88d7e-108">Prerequisites</span></span>
<span data-ttu-id="88d7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88d7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88d7e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="88d7e-111">Permission type</span></span>|<span data-ttu-id="88d7e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88d7e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88d7e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88d7e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="88d7e-114">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="88d7e-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="88d7e-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88d7e-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="88d7e-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="88d7e-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="88d7e-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88d7e-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="88d7e-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88d7e-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88d7e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="88d7e-119">Not supported.</span></span>|
|<span data-ttu-id="88d7e-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="88d7e-120">Application</span></span>||
| <span data-ttu-id="88d7e-121">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="88d7e-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="88d7e-122">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88d7e-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="88d7e-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="88d7e-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="88d7e-124">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88d7e-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88d7e-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88d7e-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88d7e-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="88d7e-126">Optional query parameters</span></span>
<span data-ttu-id="88d7e-127">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="88d7e-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88d7e-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="88d7e-128">Request headers</span></span>
|<span data-ttu-id="88d7e-129">标头</span><span class="sxs-lookup"><span data-stu-id="88d7e-129">Header</span></span>|<span data-ttu-id="88d7e-130">值</span><span class="sxs-lookup"><span data-stu-id="88d7e-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88d7e-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="88d7e-131">Authorization</span></span>|<span data-ttu-id="88d7e-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88d7e-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88d7e-133">接受</span><span class="sxs-lookup"><span data-stu-id="88d7e-133">Accept</span></span>|<span data-ttu-id="88d7e-134">application/json</span><span class="sxs-lookup"><span data-stu-id="88d7e-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88d7e-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="88d7e-135">Request body</span></span>
<span data-ttu-id="88d7e-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88d7e-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88d7e-137">响应</span><span class="sxs-lookup"><span data-stu-id="88d7e-137">Response</span></span>
<span data-ttu-id="88d7e-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88d7e-138">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88d7e-139">示例</span><span class="sxs-lookup"><span data-stu-id="88d7e-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="88d7e-140">请求</span><span class="sxs-lookup"><span data-stu-id="88d7e-140">Request</span></span>
<span data-ttu-id="88d7e-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88d7e-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="88d7e-142">响应</span><span class="sxs-lookup"><span data-stu-id="88d7e-142">Response</span></span>
<span data-ttu-id="88d7e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88d7e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2944

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
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
    "allowedOutboundClipboardSharingExceptionLength": 14,
    "notificationRestriction": "blockOrganizationalData",
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
    "filterOpenInToOnlyManagedApps": true,
    "disableProtectionOfManagedOutboundOpenInData": true,
    "protectInboundDataFromUnknownSources": true,
    "customBrowserProtocol": "Custom Browser Protocol value"
  }
}
```







