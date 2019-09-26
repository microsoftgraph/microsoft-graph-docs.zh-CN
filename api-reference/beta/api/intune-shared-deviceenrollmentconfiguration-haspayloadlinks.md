---
title: hasPayloadLinks 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b2764202c2623274a14c4e1df178aff1e38d4cdb
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199763"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="5113a-103">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="5113a-103">hasPayloadLinks action</span></span>

> <span data-ttu-id="5113a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5113a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5113a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5113a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5113a-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5113a-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5113a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5113a-107">Prerequisites</span></span>
<span data-ttu-id="5113a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5113a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5113a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5113a-110">Permission type</span></span>|<span data-ttu-id="5113a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5113a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5113a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5113a-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5113a-113">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="5113a-113">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="5113a-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5113a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5113a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5113a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5113a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5113a-116">Not supported.</span></span>|
|<span data-ttu-id="5113a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5113a-117">Application</span></span>||
| <span data-ttu-id="5113a-118">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="5113a-118">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="5113a-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5113a-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5113a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5113a-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="5113a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5113a-121">Request headers</span></span>
|<span data-ttu-id="5113a-122">标头</span><span class="sxs-lookup"><span data-stu-id="5113a-122">Header</span></span>|<span data-ttu-id="5113a-123">值</span><span class="sxs-lookup"><span data-stu-id="5113a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5113a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5113a-124">Authorization</span></span>|<span data-ttu-id="5113a-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5113a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5113a-126">接受</span><span class="sxs-lookup"><span data-stu-id="5113a-126">Accept</span></span>|<span data-ttu-id="5113a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5113a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5113a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5113a-128">Request body</span></span>
<span data-ttu-id="5113a-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5113a-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5113a-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="5113a-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5113a-131">属性</span><span class="sxs-lookup"><span data-stu-id="5113a-131">Property</span></span>|<span data-ttu-id="5113a-132">类型</span><span class="sxs-lookup"><span data-stu-id="5113a-132">Type</span></span>|<span data-ttu-id="5113a-133">说明</span><span class="sxs-lookup"><span data-stu-id="5113a-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5113a-134">payloadIds</span><span class="sxs-lookup"><span data-stu-id="5113a-134">payloadIds</span></span>|<span data-ttu-id="5113a-135">String collection</span><span class="sxs-lookup"><span data-stu-id="5113a-135">String collection</span></span>|<span data-ttu-id="5113a-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5113a-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5113a-137">响应</span><span class="sxs-lookup"><span data-stu-id="5113a-137">Response</span></span>
<span data-ttu-id="5113a-138">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合。</span><span class="sxs-lookup"><span data-stu-id="5113a-138">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5113a-139">示例</span><span class="sxs-lookup"><span data-stu-id="5113a-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="5113a-140">请求</span><span class="sxs-lookup"><span data-stu-id="5113a-140">Request</span></span>
<span data-ttu-id="5113a-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5113a-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/hasPayloadLinks

Content-type: application/json
Content-length: 53

{
  "payloadIds": [
    "Payload Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="5113a-142">响应</span><span class="sxs-lookup"><span data-stu-id="5113a-142">Response</span></span>
<span data-ttu-id="5113a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5113a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.hasPayloadLinkResultItem",
      "payloadId": "Payload Id value",
      "hasLink": true,
      "error": "Error value",
      "sources": [
        "policySets"
      ]
    }
  ]
}
```




