---
title: 调用： updateMetadata
description: 更新与调用相关联的 appliation 的元数据。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b4d4b0fc986952f7bcfdbaff09aee60609337da1
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912795"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="b4801-103">调用： updateMetadata</span><span class="sxs-lookup"><span data-stu-id="b4801-103">call: updateMetadata</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4801-104">更新与调用相关联的 appliation 的元数据。</span><span class="sxs-lookup"><span data-stu-id="b4801-104">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4801-105">权限</span><span class="sxs-lookup"><span data-stu-id="b4801-105">Permissions</span></span>
<span data-ttu-id="b4801-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4801-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4801-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4801-108">Permission type</span></span>                        | <span data-ttu-id="b4801-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4801-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b4801-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4801-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4801-111">不支持</span><span class="sxs-lookup"><span data-stu-id="b4801-111">Not Supported</span></span>                               |
| <span data-ttu-id="b4801-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4801-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4801-113">不支持</span><span class="sxs-lookup"><span data-stu-id="b4801-113">Not Supported</span></span>                               |
| <span data-ttu-id="b4801-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4801-114">Application</span></span>     | <span data-ttu-id="b4801-115">JoinGroupCallsasGuest、JoinGroupCalls、InitiateGroupCalls 和。 All</span><span class="sxs-lookup"><span data-stu-id="b4801-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4801-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4801-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /communications/calls/{id}/updateMetadata
```
> <span data-ttu-id="b4801-117">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="b4801-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="b4801-118">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="b4801-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4801-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4801-119">Request headers</span></span>
| <span data-ttu-id="b4801-120">名称</span><span class="sxs-lookup"><span data-stu-id="b4801-120">Name</span></span>          | <span data-ttu-id="b4801-121">说明</span><span class="sxs-lookup"><span data-stu-id="b4801-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b4801-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4801-122">Authorization</span></span> | <span data-ttu-id="b4801-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4801-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4801-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4801-125">Request body</span></span>
<span data-ttu-id="b4801-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b4801-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b4801-127">参数</span><span class="sxs-lookup"><span data-stu-id="b4801-127">Parameter</span></span>      | <span data-ttu-id="b4801-128">类型</span><span class="sxs-lookup"><span data-stu-id="b4801-128">Type</span></span>    |<span data-ttu-id="b4801-129">说明</span><span class="sxs-lookup"><span data-stu-id="b4801-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4801-130">metadata</span><span class="sxs-lookup"><span data-stu-id="b4801-130">metadata</span></span>|<span data-ttu-id="b4801-131">String</span><span class="sxs-lookup"><span data-stu-id="b4801-131">String</span></span>|<span data-ttu-id="b4801-132">名单中参与者提供的数据的 blob。</span><span class="sxs-lookup"><span data-stu-id="b4801-132">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="b4801-133">适用</span><span class="sxs-lookup"><span data-stu-id="b4801-133">clientContext</span></span>|<span data-ttu-id="b4801-134">String</span><span class="sxs-lookup"><span data-stu-id="b4801-134">String</span></span>|<span data-ttu-id="b4801-135">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="b4801-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="b4801-136">响应</span><span class="sxs-lookup"><span data-stu-id="b4801-136">Response</span></span>
<span data-ttu-id="b4801-137">返回`202 Accepted`响应代码和位置标头，其中包含为此请求创建的[commsOperation](../resources/commsoperation.md)的 uri。</span><span class="sxs-lookup"><span data-stu-id="b4801-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="b4801-138">示例</span><span class="sxs-lookup"><span data-stu-id="b4801-138">Example</span></span>
<span data-ttu-id="b4801-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b4801-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b4801-140">请求</span><span class="sxs-lookup"><span data-stu-id="b4801-140">Request</span></span>
<span data-ttu-id="b4801-141">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4801-141">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b4801-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4801-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b4801-143">C#</span><span class="sxs-lookup"><span data-stu-id="b4801-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updatemetadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4801-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4801-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updatemetadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b4801-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4801-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updatemetadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b4801-146">响应</span><span class="sxs-lookup"><span data-stu-id="b4801-146">Response</span></span>

> <span data-ttu-id="b4801-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b4801-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
