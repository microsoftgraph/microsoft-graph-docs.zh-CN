---
title: 调用： updateMetadata
description: 更新与调用相关联的 appliation 的元数据。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 793639bed1288dd6873a6f2b4afba53efba9e533
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440701"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="726ca-103">调用： updateMetadata</span><span class="sxs-lookup"><span data-stu-id="726ca-103">call: updateMetadata</span></span>

<span data-ttu-id="726ca-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="726ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="726ca-105">更新与调用相关联的 appliation 的元数据。</span><span class="sxs-lookup"><span data-stu-id="726ca-105">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="726ca-106">权限</span><span class="sxs-lookup"><span data-stu-id="726ca-106">Permissions</span></span>
<span data-ttu-id="726ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="726ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="726ca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="726ca-109">Permission type</span></span>                        | <span data-ttu-id="726ca-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="726ca-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="726ca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="726ca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="726ca-112">不支持</span><span class="sxs-lookup"><span data-stu-id="726ca-112">Not Supported</span></span>                               |
| <span data-ttu-id="726ca-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="726ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="726ca-114">不支持</span><span class="sxs-lookup"><span data-stu-id="726ca-114">Not Supported</span></span>                               |
| <span data-ttu-id="726ca-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="726ca-115">Application</span></span>     | <span data-ttu-id="726ca-116">JoinGroupCallsasGuest、JoinGroupCalls、InitiateGroupCalls 和。 All</span><span class="sxs-lookup"><span data-stu-id="726ca-116">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="726ca-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="726ca-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /communications/calls/{id}/updateMetadata
```
> <span data-ttu-id="726ca-118">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="726ca-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="726ca-119">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="726ca-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="726ca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="726ca-120">Request headers</span></span>
| <span data-ttu-id="726ca-121">名称</span><span class="sxs-lookup"><span data-stu-id="726ca-121">Name</span></span>          | <span data-ttu-id="726ca-122">说明</span><span class="sxs-lookup"><span data-stu-id="726ca-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="726ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="726ca-123">Authorization</span></span> | <span data-ttu-id="726ca-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="726ca-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="726ca-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="726ca-126">Request body</span></span>
<span data-ttu-id="726ca-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="726ca-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="726ca-128">参数</span><span class="sxs-lookup"><span data-stu-id="726ca-128">Parameter</span></span>      | <span data-ttu-id="726ca-129">类型</span><span class="sxs-lookup"><span data-stu-id="726ca-129">Type</span></span>    |<span data-ttu-id="726ca-130">说明</span><span class="sxs-lookup"><span data-stu-id="726ca-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="726ca-131">metadata</span><span class="sxs-lookup"><span data-stu-id="726ca-131">metadata</span></span>|<span data-ttu-id="726ca-132">String</span><span class="sxs-lookup"><span data-stu-id="726ca-132">String</span></span>|<span data-ttu-id="726ca-133">名单中参与者提供的数据的 blob。</span><span class="sxs-lookup"><span data-stu-id="726ca-133">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="726ca-134">适用</span><span class="sxs-lookup"><span data-stu-id="726ca-134">clientContext</span></span>|<span data-ttu-id="726ca-135">String</span><span class="sxs-lookup"><span data-stu-id="726ca-135">String</span></span>|<span data-ttu-id="726ca-136">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="726ca-136">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="726ca-137">响应</span><span class="sxs-lookup"><span data-stu-id="726ca-137">Response</span></span>
<span data-ttu-id="726ca-138">返回`202 Accepted`响应代码和位置标头，其中包含为此请求创建的[commsOperation](../resources/commsoperation.md)的 uri。</span><span class="sxs-lookup"><span data-stu-id="726ca-138">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="726ca-139">示例</span><span class="sxs-lookup"><span data-stu-id="726ca-139">Example</span></span>
<span data-ttu-id="726ca-140">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="726ca-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="726ca-141">请求</span><span class="sxs-lookup"><span data-stu-id="726ca-141">Request</span></span>
<span data-ttu-id="726ca-142">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="726ca-142">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="726ca-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="726ca-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-updateMetadata"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/updateMetadata
Content-Type: application/json
Content-Length: 79

{
  "metadata": "metadata-value",
  "clientContext": "clientContext-value"
}
```
# <a name="c"></a>[<span data-ttu-id="726ca-144">C#</span><span class="sxs-lookup"><span data-stu-id="726ca-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updatemetadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="726ca-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="726ca-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updatemetadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="726ca-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="726ca-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updatemetadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="726ca-147">响应</span><span class="sxs-lookup"><span data-stu-id="726ca-147">Response</span></span>

> <span data-ttu-id="726ca-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="726ca-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-updateMetadata",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.commsOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: updateMetadata",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
