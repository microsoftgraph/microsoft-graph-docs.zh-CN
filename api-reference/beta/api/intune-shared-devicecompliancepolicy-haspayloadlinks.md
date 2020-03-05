---
title: hasPayloadLinks 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aca08815a975a105938d146706070b0447444b75
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458768"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="ea027-103">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="ea027-103">hasPayloadLinks action</span></span>

<span data-ttu-id="ea027-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ea027-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea027-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea027-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea027-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea027-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea027-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ea027-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea027-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ea027-108">Prerequisites</span></span>
<span data-ttu-id="ea027-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea027-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea027-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea027-111">Permission type</span></span>|<span data-ttu-id="ea027-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ea027-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea027-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea027-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ea027-114">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="ea027-114">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ea027-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea027-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ea027-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea027-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea027-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea027-117">Not supported.</span></span>|
|<span data-ttu-id="ea027-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea027-118">Application</span></span>||
| <span data-ttu-id="ea027-119">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="ea027-119">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ea027-120">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea027-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea027-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea027-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="ea027-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea027-122">Request headers</span></span>
|<span data-ttu-id="ea027-123">标头</span><span class="sxs-lookup"><span data-stu-id="ea027-123">Header</span></span>|<span data-ttu-id="ea027-124">值</span><span class="sxs-lookup"><span data-stu-id="ea027-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea027-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea027-125">Authorization</span></span>|<span data-ttu-id="ea027-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ea027-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea027-127">接受</span><span class="sxs-lookup"><span data-stu-id="ea027-127">Accept</span></span>|<span data-ttu-id="ea027-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ea027-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea027-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea027-129">Request body</span></span>
<span data-ttu-id="ea027-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea027-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ea027-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="ea027-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ea027-132">属性</span><span class="sxs-lookup"><span data-stu-id="ea027-132">Property</span></span>|<span data-ttu-id="ea027-133">类型</span><span class="sxs-lookup"><span data-stu-id="ea027-133">Type</span></span>|<span data-ttu-id="ea027-134">说明</span><span class="sxs-lookup"><span data-stu-id="ea027-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea027-135">payloadIds</span><span class="sxs-lookup"><span data-stu-id="ea027-135">payloadIds</span></span>|<span data-ttu-id="ea027-136">String collection</span><span class="sxs-lookup"><span data-stu-id="ea027-136">String collection</span></span>|<span data-ttu-id="ea027-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ea027-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ea027-138">响应</span><span class="sxs-lookup"><span data-stu-id="ea027-138">Response</span></span>
<span data-ttu-id="ea027-139">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合。</span><span class="sxs-lookup"><span data-stu-id="ea027-139">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea027-140">示例</span><span class="sxs-lookup"><span data-stu-id="ea027-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea027-141">请求</span><span class="sxs-lookup"><span data-stu-id="ea027-141">Request</span></span>
<span data-ttu-id="ea027-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea027-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/hasPayloadLinks

Content-type: application/json
Content-length: 53

{
  "payloadIds": [
    "Payload Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ea027-143">响应</span><span class="sxs-lookup"><span data-stu-id="ea027-143">Response</span></span>
<span data-ttu-id="ea027-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea027-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








