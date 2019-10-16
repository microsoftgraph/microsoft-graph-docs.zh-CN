---
title: 列出 macOSMicrosoftEdgeApps
description: 列出 macOSMicrosoftEdgeApp 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10dbb46345415f9f841ec8f74f7ebbb39a447aab
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535322"
---
# <a name="list-macosmicrosoftedgeapps"></a><span data-ttu-id="1ee69-103">列出 macOSMicrosoftEdgeApps</span><span class="sxs-lookup"><span data-stu-id="1ee69-103">List macOSMicrosoftEdgeApps</span></span>

> <span data-ttu-id="1ee69-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1ee69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ee69-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ee69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ee69-106">列出[macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1ee69-106">List properties and relationships of the [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ee69-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1ee69-107">Prerequisites</span></span>
<span data-ttu-id="1ee69-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ee69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ee69-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ee69-110">Permission type</span></span>|<span data-ttu-id="1ee69-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1ee69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ee69-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ee69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ee69-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ee69-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1ee69-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ee69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ee69-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ee69-115">Not supported.</span></span>|
|<span data-ttu-id="1ee69-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ee69-116">Application</span></span>|<span data-ttu-id="1ee69-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ee69-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ee69-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ee69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1ee69-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ee69-119">Request headers</span></span>
|<span data-ttu-id="1ee69-120">标头</span><span class="sxs-lookup"><span data-stu-id="1ee69-120">Header</span></span>|<span data-ttu-id="1ee69-121">值</span><span class="sxs-lookup"><span data-stu-id="1ee69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ee69-122">授权</span><span class="sxs-lookup"><span data-stu-id="1ee69-122">Authorization</span></span>|<span data-ttu-id="1ee69-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1ee69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ee69-124">接受</span><span class="sxs-lookup"><span data-stu-id="1ee69-124">Accept</span></span>|<span data-ttu-id="1ee69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ee69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ee69-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ee69-126">Request body</span></span>
<span data-ttu-id="1ee69-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ee69-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ee69-128">响应</span><span class="sxs-lookup"><span data-stu-id="1ee69-128">Response</span></span>
<span data-ttu-id="1ee69-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="1ee69-129">If successful, this method returns a `200 OK` response code and a collection of [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ee69-130">示例</span><span class="sxs-lookup"><span data-stu-id="1ee69-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ee69-131">请求</span><span class="sxs-lookup"><span data-stu-id="1ee69-131">Request</span></span>
<span data-ttu-id="1ee69-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ee69-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="1ee69-133">响应</span><span class="sxs-lookup"><span data-stu-id="1ee69-133">Response</span></span>
<span data-ttu-id="1ee69-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1ee69-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1025

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSMicrosoftEdgeApp",
      "id": "c964092a-092a-c964-2a09-64c92a0964c9",
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
      "dependentAppCount": 1
    }
  ]
}
```






