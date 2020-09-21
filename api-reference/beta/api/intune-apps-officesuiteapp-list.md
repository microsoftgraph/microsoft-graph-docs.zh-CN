---
title: 列出 officeSuiteApps
description: 列出 officeSuiteApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: acbf218d265bc3756fa34292e6d4cd572c0cb171
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976926"
---
# <a name="list-officesuiteapps"></a><span data-ttu-id="db326-103">列出 officeSuiteApps</span><span class="sxs-lookup"><span data-stu-id="db326-103">List officeSuiteApps</span></span>

<span data-ttu-id="db326-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db326-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db326-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db326-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db326-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db326-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db326-107">列出 [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="db326-107">List properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db326-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="db326-108">Prerequisites</span></span>
<span data-ttu-id="db326-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db326-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db326-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="db326-111">Permission type</span></span>|<span data-ttu-id="db326-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db326-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db326-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db326-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db326-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="db326-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="db326-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db326-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db326-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="db326-116">Not supported.</span></span>|
|<span data-ttu-id="db326-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="db326-117">Application</span></span>|<span data-ttu-id="db326-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="db326-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db326-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db326-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="db326-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="db326-120">Request headers</span></span>
|<span data-ttu-id="db326-121">标头</span><span class="sxs-lookup"><span data-stu-id="db326-121">Header</span></span>|<span data-ttu-id="db326-122">值</span><span class="sxs-lookup"><span data-stu-id="db326-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db326-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db326-123">Authorization</span></span>|<span data-ttu-id="db326-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db326-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db326-125">接受</span><span class="sxs-lookup"><span data-stu-id="db326-125">Accept</span></span>|<span data-ttu-id="db326-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db326-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db326-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="db326-127">Request body</span></span>
<span data-ttu-id="db326-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db326-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db326-129">响应</span><span class="sxs-lookup"><span data-stu-id="db326-129">Response</span></span>
<span data-ttu-id="db326-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="db326-130">If successful, this method returns a `200 OK` response code and a collection of [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db326-131">示例</span><span class="sxs-lookup"><span data-stu-id="db326-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="db326-132">请求</span><span class="sxs-lookup"><span data-stu-id="db326-132">Request</span></span>
<span data-ttu-id="db326-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db326-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="db326-134">响应</span><span class="sxs-lookup"><span data-stu-id="db326-134">Response</span></span>
<span data-ttu-id="db326-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db326-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2120

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeSuiteApp",
      "id": "9b263b46-3b46-9b26-463b-269b463b269b",
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
      "supersedingAppCount": 3,
      "supersededAppCount": 2,
      "autoAcceptEula": true,
      "productIds": [
        "o365BusinessRetail"
      ],
      "excludedApps": {
        "@odata.type": "microsoft.graph.excludedApps",
        "access": true,
        "bing": true,
        "excel": true,
        "groove": true,
        "infoPath": true,
        "lync": true,
        "oneDrive": true,
        "oneNote": true,
        "outlook": true,
        "powerPoint": true,
        "publisher": true,
        "sharePointDesigner": true,
        "teams": true,
        "visio": true,
        "word": true
      },
      "useSharedComputerActivation": true,
      "updateChannel": "current",
      "officePlatformArchitecture": "x86",
      "localesToInstall": [
        "Locales To Install value"
      ],
      "installProgressDisplayLevel": "full",
      "shouldUninstallOlderVersionsOfOffice": true,
      "targetVersion": "Target Version value",
      "updateVersion": "Update Version value",
      "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
    }
  ]
}
```






