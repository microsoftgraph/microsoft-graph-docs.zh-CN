---
title: 列出 windowsPhone81GeneralConfigurations
description: 列出 windowsPhone81GeneralConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47ddf7b623f92dd88693f3e6e2f93d46d7446524
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975978"
---
# <a name="list-windowsphone81generalconfigurations"></a><span data-ttu-id="6541b-103">列出 windowsPhone81GeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="6541b-103">List windowsPhone81GeneralConfigurations</span></span>

> <span data-ttu-id="6541b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6541b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6541b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6541b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6541b-106">列出 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6541b-106">List properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6541b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6541b-107">Prerequisites</span></span>
<span data-ttu-id="6541b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6541b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6541b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6541b-110">Permission type</span></span>|<span data-ttu-id="6541b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6541b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6541b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6541b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6541b-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6541b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6541b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6541b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6541b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6541b-115">Not supported.</span></span>|
|<span data-ttu-id="6541b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6541b-116">Application</span></span>|<span data-ttu-id="6541b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6541b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6541b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6541b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6541b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6541b-119">Request headers</span></span>
|<span data-ttu-id="6541b-120">标头</span><span class="sxs-lookup"><span data-stu-id="6541b-120">Header</span></span>|<span data-ttu-id="6541b-121">值</span><span class="sxs-lookup"><span data-stu-id="6541b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6541b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6541b-122">Authorization</span></span>|<span data-ttu-id="6541b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6541b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6541b-124">接受</span><span class="sxs-lookup"><span data-stu-id="6541b-124">Accept</span></span>|<span data-ttu-id="6541b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6541b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6541b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6541b-126">Request body</span></span>
<span data-ttu-id="6541b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6541b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6541b-128">响应</span><span class="sxs-lookup"><span data-stu-id="6541b-128">Response</span></span>
<span data-ttu-id="6541b-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6541b-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6541b-130">示例</span><span class="sxs-lookup"><span data-stu-id="6541b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6541b-131">请求</span><span class="sxs-lookup"><span data-stu-id="6541b-131">Request</span></span>
<span data-ttu-id="6541b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6541b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="6541b-133">响应</span><span class="sxs-lookup"><span data-stu-id="6541b-133">Response</span></span>
<span data-ttu-id="6541b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6541b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1950

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
      "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "applyOnlyToWindowsPhone81": true,
      "appsBlockCopyPaste": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "cellularBlockWifiTethering": true,
      "compliantAppsList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "compliantAppListType": "appsInListCompliant",
      "diagnosticDataBlockSubmission": true,
      "emailBlockAddingAccounts": true,
      "locationServicesBlocked": true,
      "microsoftAccountBlocked": true,
      "nfcBlocked": true,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordMinimumCharacterSetCount": 0,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "alphanumeric",
      "passwordRequired": true,
      "screenCaptureBlocked": true,
      "storageBlockRemovableStorage": true,
      "storageRequireEncryption": true,
      "webBrowserBlocked": true,
      "wifiBlocked": true,
      "wifiBlockAutomaticConnectHotspots": true,
      "wifiBlockHotspotReporting": true,
      "windowsStoreBlocked": true
    }
  ]
}
```




