---
title: getTopMobileApps 函数
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd77e9ef52131844f46f4551e882f289ebcc345f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800779"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="076a2-103">getTopMobileApps 函数</span><span class="sxs-lookup"><span data-stu-id="076a2-103">getTopMobileApps function</span></span>

> <span data-ttu-id="076a2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="076a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="076a2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="076a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="076a2-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="076a2-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="076a2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="076a2-107">Prerequisites</span></span>
<span data-ttu-id="076a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="076a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="076a2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="076a2-110">Permission type</span></span>|<span data-ttu-id="076a2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="076a2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="076a2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="076a2-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="076a2-113">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="076a2-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="076a2-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="076a2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="076a2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="076a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="076a2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="076a2-116">Not supported.</span></span>|
|<span data-ttu-id="076a2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="076a2-117">Application</span></span>||
| <span data-ttu-id="076a2-118">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="076a2-118">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="076a2-119">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="076a2-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="076a2-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="076a2-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="076a2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="076a2-121">Request headers</span></span>
|<span data-ttu-id="076a2-122">标头</span><span class="sxs-lookup"><span data-stu-id="076a2-122">Header</span></span>|<span data-ttu-id="076a2-123">值</span><span class="sxs-lookup"><span data-stu-id="076a2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="076a2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="076a2-124">Authorization</span></span>|<span data-ttu-id="076a2-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="076a2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="076a2-126">接受</span><span class="sxs-lookup"><span data-stu-id="076a2-126">Accept</span></span>|<span data-ttu-id="076a2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="076a2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="076a2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="076a2-128">Request body</span></span>
<span data-ttu-id="076a2-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="076a2-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="076a2-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="076a2-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="076a2-131">属性</span><span class="sxs-lookup"><span data-stu-id="076a2-131">Property</span></span>|<span data-ttu-id="076a2-132">类型</span><span class="sxs-lookup"><span data-stu-id="076a2-132">Type</span></span>|<span data-ttu-id="076a2-133">说明</span><span class="sxs-lookup"><span data-stu-id="076a2-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="076a2-134">状态</span><span class="sxs-lookup"><span data-stu-id="076a2-134">status</span></span>|<span data-ttu-id="076a2-135">String</span><span class="sxs-lookup"><span data-stu-id="076a2-135">String</span></span>|<span data-ttu-id="076a2-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="076a2-136">Not yet documented</span></span>|
|<span data-ttu-id="076a2-137">count</span><span class="sxs-lookup"><span data-stu-id="076a2-137">count</span></span>|<span data-ttu-id="076a2-138">Int64</span><span class="sxs-lookup"><span data-stu-id="076a2-138">Int64</span></span>|<span data-ttu-id="076a2-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="076a2-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="076a2-140">响应</span><span class="sxs-lookup"><span data-stu-id="076a2-140">Response</span></span>
<span data-ttu-id="076a2-141">如果成功，此函数会在`200 OK`响应正文中返回响应代码和[mobileApp](../resources/intune-shared-mobileapp.md)集合。</span><span class="sxs-lookup"><span data-stu-id="076a2-141">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-shared-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="076a2-142">示例</span><span class="sxs-lookup"><span data-stu-id="076a2-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="076a2-143">请求</span><span class="sxs-lookup"><span data-stu-id="076a2-143">Request</span></span>
<span data-ttu-id="076a2-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="076a2-144">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="076a2-145">响应</span><span class="sxs-lookup"><span data-stu-id="076a2-145">Response</span></span>
<span data-ttu-id="076a2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="076a2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







