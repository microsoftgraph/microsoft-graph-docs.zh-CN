---
title: 呼叫： updateMetadata
description: 更新应用程序的元数据与呼叫相关联。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 2b736c56a7a517f0b68d656ab96933a34cf4a09d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813585"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="23c2e-103">呼叫： updateMetadata</span><span class="sxs-lookup"><span data-stu-id="23c2e-103">call: updateMetadata</span></span>

> <span data-ttu-id="23c2e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="23c2e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23c2e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="23c2e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23c2e-106">更新应用程序的元数据与呼叫相关联。</span><span class="sxs-lookup"><span data-stu-id="23c2e-106">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="23c2e-107">权限</span><span class="sxs-lookup"><span data-stu-id="23c2e-107">Permissions</span></span>
<span data-ttu-id="23c2e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23c2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23c2e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="23c2e-110">Permission type</span></span>                        | <span data-ttu-id="23c2e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23c2e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="23c2e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23c2e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="23c2e-113">不支持</span><span class="sxs-lookup"><span data-stu-id="23c2e-113">Not Supported</span></span>                               |
| <span data-ttu-id="23c2e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23c2e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23c2e-115">不支持</span><span class="sxs-lookup"><span data-stu-id="23c2e-115">Not Supported</span></span>                               |
| <span data-ttu-id="23c2e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="23c2e-116">Application</span></span>     | <span data-ttu-id="23c2e-117">Calls.JoinGroupCallsasGuest.All，Calls.JoinGroupCalls.All，Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="23c2e-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23c2e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23c2e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /applications/{id}/calls/{id}/updateMetadata
```

## <a name="request-headers"></a><span data-ttu-id="23c2e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="23c2e-119">Request headers</span></span>
| <span data-ttu-id="23c2e-120">名称</span><span class="sxs-lookup"><span data-stu-id="23c2e-120">Name</span></span>          | <span data-ttu-id="23c2e-121">说明</span><span class="sxs-lookup"><span data-stu-id="23c2e-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="23c2e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="23c2e-122">Authorization</span></span> | <span data-ttu-id="23c2e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="23c2e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23c2e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="23c2e-125">Request body</span></span>
<span data-ttu-id="23c2e-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="23c2e-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="23c2e-127">参数</span><span class="sxs-lookup"><span data-stu-id="23c2e-127">Parameter</span></span>      | <span data-ttu-id="23c2e-128">类型</span><span class="sxs-lookup"><span data-stu-id="23c2e-128">Type</span></span>    |<span data-ttu-id="23c2e-129">Description</span><span class="sxs-lookup"><span data-stu-id="23c2e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23c2e-130">元数据</span><span class="sxs-lookup"><span data-stu-id="23c2e-130">metadata</span></span>|<span data-ttu-id="23c2e-131">字符串</span><span class="sxs-lookup"><span data-stu-id="23c2e-131">String</span></span>|<span data-ttu-id="23c2e-132">提供在名单中的参与者的数据的 blob。</span><span class="sxs-lookup"><span data-stu-id="23c2e-132">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="23c2e-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="23c2e-133">clientContext</span></span>|<span data-ttu-id="23c2e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="23c2e-134">String</span></span>|<span data-ttu-id="23c2e-135">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="23c2e-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="23c2e-136">响应</span><span class="sxs-lookup"><span data-stu-id="23c2e-136">Response</span></span>
<span data-ttu-id="23c2e-137">返回`202 Accepted`响应代码和具有[commsOperation](../resources/commsoperation.md)创建的此请求 uri 中的位置标头。</span><span class="sxs-lookup"><span data-stu-id="23c2e-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="23c2e-138">示例</span><span class="sxs-lookup"><span data-stu-id="23c2e-138">Example</span></span>
<span data-ttu-id="23c2e-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="23c2e-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="23c2e-140">请求</span><span class="sxs-lookup"><span data-stu-id="23c2e-140">Request</span></span>
<span data-ttu-id="23c2e-141">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="23c2e-141">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-updateMetadata"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/updateMetadata
Content-Type: application/json
Content-Length: 79

{
  "metadata": "metadata-value",
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="23c2e-142">响应</span><span class="sxs-lookup"><span data-stu-id="23c2e-142">Response</span></span>

> <span data-ttu-id="23c2e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="23c2e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: updateMetadata",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
