---
title: 列表答复
description: 检索了 chatmessage 对象的列表。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a6622bc7859ae8118a129c555349f391891f9c1a
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718396"
---
# <a name="list-replies"></a><span data-ttu-id="b107a-103">列表答复</span><span class="sxs-lookup"><span data-stu-id="b107a-103">List replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b107a-104">检索了 chatmessage 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="b107a-104">Retrieve a list of chatmessage objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b107a-105">权限</span><span class="sxs-lookup"><span data-stu-id="b107a-105">Permissions</span></span>

<span data-ttu-id="b107a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b107a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b107a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b107a-108">Permission type</span></span>                        | <span data-ttu-id="b107a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b107a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b107a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b107a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b107a-111">聊天、阅读和读写</span><span class="sxs-lookup"><span data-stu-id="b107a-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="b107a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b107a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b107a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b107a-113">Not supported.</span></span> |
| <span data-ttu-id="b107a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b107a-114">Application</span></span>                            | <span data-ttu-id="b107a-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="b107a-115">Chat.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="b107a-116">在使用应用程序权限调用此 API 之前, 您必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="b107a-116">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="b107a-117">有关详细信息, 请参阅[Microsoft 团队中的受保护 api](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="b107a-117">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="b107a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b107a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/replies
GET /users/{id}/chats/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b107a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b107a-119">Optional query parameters</span></span>

<span data-ttu-id="b107a-120">此操作不支持[OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b107a-120">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b107a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b107a-121">Request headers</span></span>

| <span data-ttu-id="b107a-122">名称</span><span class="sxs-lookup"><span data-stu-id="b107a-122">Name</span></span>      |<span data-ttu-id="b107a-123">说明</span><span class="sxs-lookup"><span data-stu-id="b107a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b107a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b107a-124">Authorization</span></span> | <span data-ttu-id="b107a-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b107a-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b107a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b107a-126">Request body</span></span>

<span data-ttu-id="b107a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b107a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b107a-128">响应</span><span class="sxs-lookup"><span data-stu-id="b107a-128">Response</span></span>

<span data-ttu-id="b107a-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatMessage](../resources/chatmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b107a-129">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b107a-130">示例</span><span class="sxs-lookup"><span data-stu-id="b107a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b107a-131">请求</span><span class="sxs-lookup"><span data-stu-id="b107a-131">Request</span></span>

<span data-ttu-id="b107a-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b107a-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b107a-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b107a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/replies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b107a-134">C#</span><span class="sxs-lookup"><span data-stu-id="b107a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b107a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b107a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b107a-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="b107a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b107a-137">响应</span><span class="sxs-lookup"><span data-stu-id="b107a-137">Response</span></span>

<span data-ttu-id="b107a-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b107a-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b107a-139">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b107a-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b107a-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b107a-140">All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
