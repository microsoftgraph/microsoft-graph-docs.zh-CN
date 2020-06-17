---
title: 列出对话
description: 检索此组中的会话列表。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f9b4b582f0ff3b414137298c08f6582e6fe5439f
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744032"
---
# <a name="list-conversations"></a><span data-ttu-id="dbff6-103">列出对话</span><span class="sxs-lookup"><span data-stu-id="dbff6-103">List conversations</span></span>

<span data-ttu-id="dbff6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbff6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dbff6-105">检索此组中的[对话](../resources/conversation.md)列表。</span><span class="sxs-lookup"><span data-stu-id="dbff6-105">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbff6-106">权限</span><span class="sxs-lookup"><span data-stu-id="dbff6-106">Permissions</span></span>
<span data-ttu-id="dbff6-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="dbff6-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="dbff6-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbff6-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbff6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbff6-109">Permission type</span></span>      | <span data-ttu-id="dbff6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dbff6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbff6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbff6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dbff6-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbff6-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dbff6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbff6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbff6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbff6-114">Not supported.</span></span>    |
|<span data-ttu-id="dbff6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbff6-115">Application</span></span> | <span data-ttu-id="dbff6-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbff6-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbff6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbff6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dbff6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dbff6-118">Optional query parameters</span></span>
<span data-ttu-id="dbff6-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dbff6-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dbff6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dbff6-120">Request headers</span></span>
| <span data-ttu-id="dbff6-121">标头</span><span class="sxs-lookup"><span data-stu-id="dbff6-121">Header</span></span>       | <span data-ttu-id="dbff6-122">值</span><span class="sxs-lookup"><span data-stu-id="dbff6-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dbff6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbff6-123">Authorization</span></span>  | <span data-ttu-id="dbff6-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="dbff6-124">Bearer {token}.</span></span> <span data-ttu-id="dbff6-125">Required.</span><span class="sxs-lookup"><span data-stu-id="dbff6-125">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dbff6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dbff6-126">Request body</span></span>
<span data-ttu-id="dbff6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dbff6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbff6-128">响应</span><span class="sxs-lookup"><span data-stu-id="dbff6-128">Response</span></span>
<span data-ttu-id="dbff6-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Conversation](../resources/conversation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dbff6-129">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbff6-130">示例</span><span class="sxs-lookup"><span data-stu-id="dbff6-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="dbff6-131">请求</span><span class="sxs-lookup"><span data-stu-id="dbff6-131">Request</span></span>
<span data-ttu-id="dbff6-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dbff6-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dbff6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbff6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
# <a name="c"></a>[<span data-ttu-id="dbff6-134">C#</span><span class="sxs-lookup"><span data-stu-id="dbff6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbff6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbff6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbff6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbff6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dbff6-137">Java</span><span class="sxs-lookup"><span data-stu-id="dbff6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="dbff6-138">响应</span><span class="sxs-lookup"><span data-stu-id="dbff6-138">Response</span></span>
<span data-ttu-id="dbff6-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dbff6-139">The following is an example of the response.</span></span>
><span data-ttu-id="dbff6-140">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="dbff6-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dbff6-141">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="dbff6-141">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "preview": "preview-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
