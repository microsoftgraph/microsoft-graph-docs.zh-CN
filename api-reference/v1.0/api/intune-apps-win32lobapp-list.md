---
title: 列出 win32LobApps
description: 列出 win32LobApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec407801c60990bb93c802aa4682e28566d62c8b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758727"
---
# <a name="list-win32lobapps"></a><span data-ttu-id="a741e-103">列出 win32LobApps</span><span class="sxs-lookup"><span data-stu-id="a741e-103">List win32LobApps</span></span>

<span data-ttu-id="a741e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a741e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a741e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a741e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a741e-106">列出 [win32LobApp 对象的属性和](../resources/intune-apps-win32lobapp.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="a741e-106">List properties and relationships of the [win32LobApp](../resources/intune-apps-win32lobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a741e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a741e-107">Prerequisites</span></span>
<span data-ttu-id="a741e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a741e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a741e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a741e-110">Permission type</span></span>|<span data-ttu-id="a741e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a741e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a741e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a741e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a741e-113">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a741e-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a741e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a741e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a741e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a741e-115">Not supported.</span></span>|
|<span data-ttu-id="a741e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a741e-116">Application</span></span>|<span data-ttu-id="a741e-117">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a741e-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a741e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a741e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a741e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a741e-119">Request headers</span></span>
|<span data-ttu-id="a741e-120">标头</span><span class="sxs-lookup"><span data-stu-id="a741e-120">Header</span></span>|<span data-ttu-id="a741e-121">值</span><span class="sxs-lookup"><span data-stu-id="a741e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a741e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a741e-122">Authorization</span></span>|<span data-ttu-id="a741e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a741e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a741e-124">接受</span><span class="sxs-lookup"><span data-stu-id="a741e-124">Accept</span></span>|<span data-ttu-id="a741e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a741e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a741e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a741e-126">Request body</span></span>
<span data-ttu-id="a741e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a741e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a741e-128">响应</span><span class="sxs-lookup"><span data-stu-id="a741e-128">Response</span></span>
<span data-ttu-id="a741e-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [win32LobApp](../resources/intune-apps-win32lobapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a741e-129">If successful, this method returns a `200 OK` response code and a collection of [win32LobApp](../resources/intune-apps-win32lobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a741e-130">示例</span><span class="sxs-lookup"><span data-stu-id="a741e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a741e-131">请求</span><span class="sxs-lookup"><span data-stu-id="a741e-131">Request</span></span>
<span data-ttu-id="a741e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a741e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="a741e-133">响应</span><span class="sxs-lookup"><span data-stu-id="a741e-133">Response</span></span>
<span data-ttu-id="a741e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a741e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2599

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
      "publishingState": "processing",
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "installCommandLine": "Install Command Line value",
      "uninstallCommandLine": "Uninstall Command Line value",
      "applicableArchitectures": "x86",
      "minimumFreeDiskSpaceInMB": 8,
      "minimumMemoryInMB": 1,
      "minimumNumberOfProcessors": 9,
      "minimumCpuSpeedInMHz": 4,
      "rules": [
        {
          "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
          "ruleType": "requirement",
          "check32BitOn64System": true,
          "keyPath": "Key Path value",
          "valueName": "Value Name value",
          "operationType": "exists",
          "operator": "equal",
          "comparisonValue": "Comparison Value value"
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
      "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
    }
  ]
}
```




