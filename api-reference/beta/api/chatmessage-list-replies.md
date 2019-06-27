---
title: 列表答复
description: 检索了 chatmessage 对象的列表。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a79d94029a085e48677ed601795b834fc095db2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261447"
---
# <a name="list-replies"></a><span data-ttu-id="e2007-103">列表答复</span><span class="sxs-lookup"><span data-stu-id="e2007-103">List replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2007-104">检索了 chatmessage 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e2007-104">Retrieve a list of chatmessage objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2007-105">权限</span><span class="sxs-lookup"><span data-stu-id="e2007-105">Permissions</span></span>

<span data-ttu-id="e2007-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2007-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e2007-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2007-108">Permission type</span></span>                        | <span data-ttu-id="e2007-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2007-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e2007-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2007-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2007-111">聊天、阅读和读写</span><span class="sxs-lookup"><span data-stu-id="e2007-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="e2007-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2007-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2007-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2007-113">Not supported.</span></span> |
| <span data-ttu-id="e2007-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2007-114">Application</span></span>                            | <span data-ttu-id="e2007-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2007-115">Chat.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2007-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2007-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/replies
GET /users/{id}/chats/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2007-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e2007-117">Optional query parameters</span></span>

<span data-ttu-id="e2007-118">此操作不支持[OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e2007-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2007-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2007-119">Request headers</span></span>

| <span data-ttu-id="e2007-120">名称</span><span class="sxs-lookup"><span data-stu-id="e2007-120">Name</span></span>      |<span data-ttu-id="e2007-121">说明</span><span class="sxs-lookup"><span data-stu-id="e2007-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e2007-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2007-122">Authorization</span></span> | <span data-ttu-id="e2007-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e2007-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2007-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2007-124">Request body</span></span>

<span data-ttu-id="e2007-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2007-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2007-126">响应</span><span class="sxs-lookup"><span data-stu-id="e2007-126">Response</span></span>

<span data-ttu-id="e2007-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatMessage](../resources/chatmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e2007-127">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e2007-128">示例</span><span class="sxs-lookup"><span data-stu-id="e2007-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e2007-129">请求</span><span class="sxs-lookup"><span data-stu-id="e2007-129">Request</span></span>

<span data-ttu-id="e2007-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e2007-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_replies"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/replies
```

### <a name="response"></a><span data-ttu-id="e2007-131">响应</span><span class="sxs-lookup"><span data-stu-id="e2007-131">Response</span></span>

<span data-ttu-id="e2007-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e2007-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="e2007-133">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e2007-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e2007-134">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e2007-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "replyToId": "replyToId-value",
      "from": {
        "application": {
          "id": "id-value",
          "displayName": "displayName-value"
        },
        "device": {
          "id": "id-value",
          "displayName": "displayName-value"
        },
        "user": {
          "id": "id-value",
          "displayName": "displayName-value"
        }
      },
      "etag": "etag-value",
      "messageType": "messageType-value",
      "createdDateTime": "datetime-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e2007-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e2007-135">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="e2007-136">C#</span><span class="sxs-lookup"><span data-stu-id="e2007-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_replies-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2007-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="e2007-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_replies-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e2007-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="e2007-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_replies-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessage-list-replies.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chatmessage-list-replies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/chatmessage-list-replies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}-->
