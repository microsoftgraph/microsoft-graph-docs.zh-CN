---
title: 列出 macOSMicrosoftEdgeApps
description: 列出 macOSMicrosoftEdgeApp 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4200be0bfe2244d60e11c4f7039b0c7d3ef2e38b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445300"
---
# <a name="list-macosmicrosoftedgeapps"></a><span data-ttu-id="71139-103">列出 macOSMicrosoftEdgeApps</span><span class="sxs-lookup"><span data-stu-id="71139-103">List macOSMicrosoftEdgeApps</span></span>

<span data-ttu-id="71139-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="71139-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71139-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="71139-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71139-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71139-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71139-107">列出[macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71139-107">List properties and relationships of the [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71139-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="71139-108">Prerequisites</span></span>
<span data-ttu-id="71139-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71139-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71139-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="71139-111">Permission type</span></span>|<span data-ttu-id="71139-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="71139-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71139-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71139-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71139-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="71139-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="71139-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71139-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71139-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="71139-116">Not supported.</span></span>|
|<span data-ttu-id="71139-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="71139-117">Application</span></span>|<span data-ttu-id="71139-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="71139-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71139-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71139-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="71139-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="71139-120">Request headers</span></span>
|<span data-ttu-id="71139-121">标头</span><span class="sxs-lookup"><span data-stu-id="71139-121">Header</span></span>|<span data-ttu-id="71139-122">值</span><span class="sxs-lookup"><span data-stu-id="71139-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71139-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71139-123">Authorization</span></span>|<span data-ttu-id="71139-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="71139-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71139-125">接受</span><span class="sxs-lookup"><span data-stu-id="71139-125">Accept</span></span>|<span data-ttu-id="71139-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71139-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71139-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="71139-127">Request body</span></span>
<span data-ttu-id="71139-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71139-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71139-129">响应</span><span class="sxs-lookup"><span data-stu-id="71139-129">Response</span></span>
<span data-ttu-id="71139-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="71139-130">If successful, this method returns a `200 OK` response code and a collection of [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71139-131">示例</span><span class="sxs-lookup"><span data-stu-id="71139-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="71139-132">请求</span><span class="sxs-lookup"><span data-stu-id="71139-132">Request</span></span>
<span data-ttu-id="71139-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71139-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="71139-134">响应</span><span class="sxs-lookup"><span data-stu-id="71139-134">Response</span></span>
<span data-ttu-id="71139-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71139-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1051

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
      "dependentAppCount": 1,
      "channel": "beta"
    }
  ]
}
```





