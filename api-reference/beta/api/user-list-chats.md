---
title: 列出聊天
description: 检索聊天对象的列表。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1dd4dee5f807f31cd9d8110be37abb14b792fdef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451887"
---
# <a name="list-chats"></a><span data-ttu-id="321a8-103">列出聊天</span><span class="sxs-lookup"><span data-stu-id="321a8-103">List chats</span></span>

<span data-ttu-id="321a8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="321a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="321a8-105">检索聊天对象的列表。</span><span class="sxs-lookup"><span data-stu-id="321a8-105">Retrieve a list of chat objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="321a8-106">权限</span><span class="sxs-lookup"><span data-stu-id="321a8-106">Permissions</span></span>

<span data-ttu-id="321a8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="321a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="321a8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="321a8-109">Permission type</span></span>                        | <span data-ttu-id="321a8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="321a8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="321a8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="321a8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="321a8-112">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="321a8-112">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="321a8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="321a8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="321a8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="321a8-114">Not supported.</span></span> |
| <span data-ttu-id="321a8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="321a8-115">Application</span></span>                            | <span data-ttu-id="321a8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="321a8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="321a8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="321a8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="321a8-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="321a8-118">Optional query parameters</span></span>

<span data-ttu-id="321a8-119">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="321a8-119">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="321a8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="321a8-120">Request headers</span></span>

| <span data-ttu-id="321a8-121">名称</span><span class="sxs-lookup"><span data-stu-id="321a8-121">Name</span></span>      |<span data-ttu-id="321a8-122">说明</span><span class="sxs-lookup"><span data-stu-id="321a8-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="321a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="321a8-123">Authorization</span></span> | <span data-ttu-id="321a8-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="321a8-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="321a8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="321a8-125">Request body</span></span>

<span data-ttu-id="321a8-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="321a8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="321a8-127">响应</span><span class="sxs-lookup"><span data-stu-id="321a8-127">Response</span></span>

<span data-ttu-id="321a8-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chat](../resources/chat.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="321a8-128">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="321a8-129">示例</span><span class="sxs-lookup"><span data-stu-id="321a8-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="321a8-130">请求</span><span class="sxs-lookup"><span data-stu-id="321a8-130">Request</span></span>

<span data-ttu-id="321a8-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="321a8-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="321a8-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="321a8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats
```
# <a name="c"></a>[<span data-ttu-id="321a8-133">C#</span><span class="sxs-lookup"><span data-stu-id="321a8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="321a8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="321a8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="321a8-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="321a8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="321a8-136">响应</span><span class="sxs-lookup"><span data-stu-id="321a8-136">Response</span></span>

<span data-ttu-id="321a8-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="321a8-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="321a8-138">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="321a8-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="321a8-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="321a8-139">All the properties will be returned from an actual call.</span></span>

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
