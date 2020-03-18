---
title: 列出 mobileApps
description: 列出 mobileApp 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d3052bf2d59a6dfc0fcd8246fa73ddb3641ef02d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800765"
---
# <a name="list-mobileapps"></a><span data-ttu-id="b2762-103">列出 mobileApps</span><span class="sxs-lookup"><span data-stu-id="b2762-103">List mobileApps</span></span>

> <span data-ttu-id="b2762-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2762-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2762-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2762-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2762-106">列出 [mobileApp](../resources/intune-shared-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b2762-106">List properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2762-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b2762-107">Prerequisites</span></span>
<span data-ttu-id="b2762-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2762-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2762-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2762-110">Permission type</span></span>|<span data-ttu-id="b2762-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b2762-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2762-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2762-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b2762-113">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="b2762-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="b2762-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2762-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="b2762-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="b2762-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b2762-116">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2762-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b2762-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2762-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2762-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2762-118">Not supported.</span></span>|
|<span data-ttu-id="b2762-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2762-119">Application</span></span>||
| <span data-ttu-id="b2762-120">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="b2762-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="b2762-121">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2762-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="b2762-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="b2762-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b2762-123">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2762-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2762-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2762-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b2762-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2762-125">Request headers</span></span>
|<span data-ttu-id="b2762-126">标头</span><span class="sxs-lookup"><span data-stu-id="b2762-126">Header</span></span>|<span data-ttu-id="b2762-127">值</span><span class="sxs-lookup"><span data-stu-id="b2762-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2762-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2762-128">Authorization</span></span>|<span data-ttu-id="b2762-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b2762-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2762-130">接受</span><span class="sxs-lookup"><span data-stu-id="b2762-130">Accept</span></span>|<span data-ttu-id="b2762-131">application/json</span><span class="sxs-lookup"><span data-stu-id="b2762-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2762-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2762-132">Request body</span></span>
<span data-ttu-id="b2762-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b2762-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2762-134">响应</span><span class="sxs-lookup"><span data-stu-id="b2762-134">Response</span></span>
<span data-ttu-id="b2762-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mobileApp](../resources/intune-shared-mobileapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b2762-135">If successful, this method returns a `200 OK` response code and a collection of [mobileApp](../resources/intune-shared-mobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2762-136">示例</span><span class="sxs-lookup"><span data-stu-id="b2762-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2762-137">请求</span><span class="sxs-lookup"><span data-stu-id="b2762-137">Request</span></span>
<span data-ttu-id="b2762-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b2762-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="b2762-139">响应</span><span class="sxs-lookup"><span data-stu-id="b2762-139">Response</span></span>
<span data-ttu-id="b2762-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2762-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1013

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileApp",
      "id": "0177548a-548a-0177-8a54-77018a547701",
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







