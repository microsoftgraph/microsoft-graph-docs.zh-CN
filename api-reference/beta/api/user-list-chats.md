---
title: 列出聊天
description: 检索聊天对象的列表。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1aabbc0facd809f8387ceb68c97fdf64c98845c1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951529"
---
# <a name="list-chats"></a><span data-ttu-id="9f71c-103">列出聊天</span><span class="sxs-lookup"><span data-stu-id="9f71c-103">List chats</span></span>

<span data-ttu-id="9f71c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f71c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f71c-105">检索聊天对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9f71c-105">Retrieve a list of chat objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f71c-106">权限</span><span class="sxs-lookup"><span data-stu-id="9f71c-106">Permissions</span></span>

<span data-ttu-id="9f71c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f71c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f71c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f71c-109">Permission type</span></span>                        | <span data-ttu-id="9f71c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f71c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9f71c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f71c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f71c-112">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f71c-112">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="9f71c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f71c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f71c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f71c-114">Not supported.</span></span> |
| <span data-ttu-id="9f71c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f71c-115">Application</span></span>                            | <span data-ttu-id="9f71c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f71c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f71c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f71c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f71c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9f71c-118">Optional query parameters</span></span>

<span data-ttu-id="9f71c-119">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9f71c-119">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f71c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f71c-120">Request headers</span></span>

| <span data-ttu-id="9f71c-121">名称</span><span class="sxs-lookup"><span data-stu-id="9f71c-121">Name</span></span>      |<span data-ttu-id="9f71c-122">说明</span><span class="sxs-lookup"><span data-stu-id="9f71c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9f71c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f71c-123">Authorization</span></span> | <span data-ttu-id="9f71c-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9f71c-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f71c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f71c-125">Request body</span></span>

<span data-ttu-id="9f71c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9f71c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f71c-127">响应</span><span class="sxs-lookup"><span data-stu-id="9f71c-127">Response</span></span>

<span data-ttu-id="9f71c-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chat](../resources/chat.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9f71c-128">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f71c-129">示例</span><span class="sxs-lookup"><span data-stu-id="9f71c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f71c-130">请求</span><span class="sxs-lookup"><span data-stu-id="9f71c-130">Request</span></span>

<span data-ttu-id="9f71c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9f71c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9f71c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f71c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats
```
# <a name="c"></a>[<span data-ttu-id="9f71c-133">C#</span><span class="sxs-lookup"><span data-stu-id="9f71c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f71c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f71c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f71c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f71c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f71c-136">Java</span><span class="sxs-lookup"><span data-stu-id="9f71c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chats-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9f71c-137">响应</span><span class="sxs-lookup"><span data-stu-id="9f71c-137">Response</span></span>

<span data-ttu-id="9f71c-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9f71c-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9f71c-139">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9f71c-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9f71c-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9f71c-140">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "topic": "topic-value",
      "createdDateTime": "datetime-value",
      "lastUpdatedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List chats",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


