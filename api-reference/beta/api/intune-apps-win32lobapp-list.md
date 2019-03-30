---
title: 列出 win32LobApps
description: 列出 win32LobApp 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8b0187b3e752ca642539a48279a9d9dce690d39
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973234"
---
# <a name="list-win32lobapps"></a><span data-ttu-id="419d1-103">列出 win32LobApps</span><span class="sxs-lookup"><span data-stu-id="419d1-103">List win32LobApps</span></span>

> <span data-ttu-id="419d1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="419d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="419d1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="419d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="419d1-106">列出[win32LobApp](../resources/intune-apps-win32lobapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="419d1-106">List properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="419d1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="419d1-107">Prerequisites</span></span>
<span data-ttu-id="419d1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="419d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="419d1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="419d1-110">Permission type</span></span>|<span data-ttu-id="419d1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="419d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="419d1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="419d1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="419d1-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="419d1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="419d1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="419d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="419d1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="419d1-115">Not supported.</span></span>|
|<span data-ttu-id="419d1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="419d1-116">Application</span></span>|<span data-ttu-id="419d1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="419d1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="419d1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="419d1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="419d1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="419d1-119">Request headers</span></span>
|<span data-ttu-id="419d1-120">标头</span><span class="sxs-lookup"><span data-stu-id="419d1-120">Header</span></span>|<span data-ttu-id="419d1-121">值</span><span class="sxs-lookup"><span data-stu-id="419d1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="419d1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="419d1-122">Authorization</span></span>|<span data-ttu-id="419d1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="419d1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="419d1-124">接受</span><span class="sxs-lookup"><span data-stu-id="419d1-124">Accept</span></span>|<span data-ttu-id="419d1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="419d1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="419d1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="419d1-126">Request body</span></span>
<span data-ttu-id="419d1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="419d1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="419d1-128">响应</span><span class="sxs-lookup"><span data-stu-id="419d1-128">Response</span></span>
<span data-ttu-id="419d1-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[win32LobApp](../resources/intune-apps-win32lobapp.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="419d1-129">If successful, this method returns a `200 OK` response code and a collection of [win32LobApp](../resources/intune-apps-win32lobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="419d1-130">示例</span><span class="sxs-lookup"><span data-stu-id="419d1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="419d1-131">请求</span><span class="sxs-lookup"><span data-stu-id="419d1-131">Request</span></span>
<span data-ttu-id="419d1-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="419d1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="419d1-133">响应</span><span class="sxs-lookup"><span data-stu-id="419d1-133">Response</span></span>
<span data-ttu-id="419d1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="419d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2877

{
  "value": [
    {
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
        "v10_1803": true
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
      "installExperience": {
        "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
        "runAsAccount": "user"
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
      "setupFilePath": "Setup File Path value"
    }
  ]
}
```




