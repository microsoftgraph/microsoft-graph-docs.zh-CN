---
title: 获取 win32LobApp
description: 读取 win32LobApp 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 185eabaf11a7256dc98c6cb57f9e43d2e86627aa
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760975"
---
# <a name="get-win32lobapp"></a><span data-ttu-id="66e56-103">获取 win32LobApp</span><span class="sxs-lookup"><span data-stu-id="66e56-103">Get win32LobApp</span></span>

> <span data-ttu-id="66e56-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66e56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66e56-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66e56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66e56-106">读取[win32LobApp](../resources/intune-apps-win32lobapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="66e56-106">Read properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66e56-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="66e56-107">Prerequisites</span></span>
<span data-ttu-id="66e56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66e56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66e56-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="66e56-110">Permission type</span></span>|<span data-ttu-id="66e56-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="66e56-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66e56-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66e56-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66e56-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="66e56-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="66e56-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66e56-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66e56-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="66e56-115">Not supported.</span></span>|
|<span data-ttu-id="66e56-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="66e56-116">Application</span></span>|<span data-ttu-id="66e56-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="66e56-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66e56-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66e56-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66e56-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="66e56-119">Optional query parameters</span></span>
<span data-ttu-id="66e56-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="66e56-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66e56-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="66e56-121">Request headers</span></span>
|<span data-ttu-id="66e56-122">标头</span><span class="sxs-lookup"><span data-stu-id="66e56-122">Header</span></span>|<span data-ttu-id="66e56-123">值</span><span class="sxs-lookup"><span data-stu-id="66e56-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66e56-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="66e56-124">Authorization</span></span>|<span data-ttu-id="66e56-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="66e56-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66e56-126">接受</span><span class="sxs-lookup"><span data-stu-id="66e56-126">Accept</span></span>|<span data-ttu-id="66e56-127">application/json</span><span class="sxs-lookup"><span data-stu-id="66e56-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66e56-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="66e56-128">Request body</span></span>
<span data-ttu-id="66e56-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="66e56-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66e56-130">响应</span><span class="sxs-lookup"><span data-stu-id="66e56-130">Response</span></span>
<span data-ttu-id="66e56-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[win32LobApp](../resources/intune-apps-win32lobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="66e56-131">If successful, this method returns a `200 OK` response code and [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66e56-132">示例</span><span class="sxs-lookup"><span data-stu-id="66e56-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="66e56-133">请求</span><span class="sxs-lookup"><span data-stu-id="66e56-133">Request</span></span>
<span data-ttu-id="66e56-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66e56-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="66e56-135">响应</span><span class="sxs-lookup"><span data-stu-id="66e56-135">Response</span></span>
<span data-ttu-id="66e56-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66e56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3242

{
  "value": {
    "@odata.type": "#microsoft.graph.win32LobApp",
    "id": "9607b530-b530-9607-30b5-079630b50796",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "uploadState": 11,
    "publishingState": "processing",
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "dependentAppCount": 1,
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "installCommandLine": "Install Command Line value",
    "uninstallCommandLine": "Uninstall Command Line value",
    "applicableArchitectures": "x86",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
      "v8_0": true,
      "v8_1": true,
      "v10_0": true,
      "v10_1607": true,
      "v10_1703": true,
      "v10_1709": true,
      "v10_1803": true,
      "v10_1809": true,
      "v10_1903": true
    },
    "minimumFreeDiskSpaceInMB": 8,
    "minimumMemoryInMB": 1,
    "minimumNumberOfProcessors": 9,
    "minimumCpuSpeedInMHz": 4,
    "detectionRules": [
      {
        "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
        "check32BitOn64System": true,
        "keyPath": "Key Path value",
        "valueName": "Value Name value",
        "detectionType": "exists",
        "operator": "equal",
        "detectionValue": "Detection Value value"
      }
    ],
    "requirementRules": [
      {
        "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
        "operator": "equal",
        "detectionValue": "Detection Value value",
        "check32BitOn64System": true,
        "keyPath": "Key Path value",
        "valueName": "Value Name value",
        "detectionType": "exists"
      }
    ],
    "installExperience": {
      "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
      "runAsAccount": "user",
      "deviceRestartBehavior": "allow"
    },
    "returnCodes": [
      {
        "@odata.type": "microsoft.graph.win32LobAppReturnCode",
        "returnCode": 10,
        "type": "success"
      }
    ],
    "msiInformation": {
      "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
      "productCode": "Product Code value",
      "productVersion": "Product Version value",
      "upgradeCode": "Upgrade Code value",
      "requiresReboot": true,
      "packageType": "perUser",
      "productName": "Product Name value",
      "publisher": "Publisher value"
    },
    "setupFilePath": "Setup File Path value",
    "installLanguage": "Install Language value"
  }
}
```




