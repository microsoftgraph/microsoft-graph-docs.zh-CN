---
title: 列出 officeSuiteApps
description: 列出 officeSuiteApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27502115c5e67bf5bf432161d95e4a22f9957b16
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793281"
---
# <a name="list-officesuiteapps"></a><span data-ttu-id="5d0a0-103">列出 officeSuiteApps</span><span class="sxs-lookup"><span data-stu-id="5d0a0-103">List officeSuiteApps</span></span>

<span data-ttu-id="5d0a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d0a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d0a0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5d0a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d0a0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5d0a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d0a0-107">列出[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5d0a0-107">List properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d0a0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5d0a0-108">Prerequisites</span></span>
<span data-ttu-id="5d0a0-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5d0a0-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5d0a0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d0a0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d0a0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d0a0-111">Permission type</span></span>|<span data-ttu-id="5d0a0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5d0a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d0a0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d0a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d0a0-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d0a0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5d0a0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d0a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d0a0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d0a0-116">Not supported.</span></span>|
|<span data-ttu-id="5d0a0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d0a0-117">Application</span></span>|<span data-ttu-id="5d0a0-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d0a0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d0a0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d0a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5d0a0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d0a0-120">Request headers</span></span>
|<span data-ttu-id="5d0a0-121">标头</span><span class="sxs-lookup"><span data-stu-id="5d0a0-121">Header</span></span>|<span data-ttu-id="5d0a0-122">值</span><span class="sxs-lookup"><span data-stu-id="5d0a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d0a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d0a0-123">Authorization</span></span>|<span data-ttu-id="5d0a0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5d0a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d0a0-125">接受</span><span class="sxs-lookup"><span data-stu-id="5d0a0-125">Accept</span></span>|<span data-ttu-id="5d0a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d0a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d0a0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d0a0-127">Request body</span></span>
<span data-ttu-id="5d0a0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5d0a0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d0a0-129">响应</span><span class="sxs-lookup"><span data-stu-id="5d0a0-129">Response</span></span>
<span data-ttu-id="5d0a0-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="5d0a0-130">If successful, this method returns a `200 OK` response code and a collection of [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d0a0-131">示例</span><span class="sxs-lookup"><span data-stu-id="5d0a0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d0a0-132">请求</span><span class="sxs-lookup"><span data-stu-id="5d0a0-132">Request</span></span>
<span data-ttu-id="5d0a0-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5d0a0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="5d0a0-134">响应</span><span class="sxs-lookup"><span data-stu-id="5d0a0-134">Response</span></span>
<span data-ttu-id="5d0a0-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="5d0a0-135">Here is an example of the response.</span></span> <span data-ttu-id="5d0a0-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="5d0a0-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5d0a0-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5d0a0-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2055

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



