---
title: 列出答复
description: 检索 chatmessage 对象的列表。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 025607cb1b2b9bb33820b8877cbde1d6a1fac844
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947795"
---
# <a name="list-replies"></a><span data-ttu-id="d3ee0-103">列出答复</span><span class="sxs-lookup"><span data-stu-id="d3ee0-103">List replies</span></span>

<span data-ttu-id="d3ee0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3ee0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3ee0-105">检索 chatmessage 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d3ee0-105">Retrieve a list of chatmessage objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3ee0-106">权限</span><span class="sxs-lookup"><span data-stu-id="d3ee0-106">Permissions</span></span>

<span data-ttu-id="d3ee0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3ee0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3ee0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3ee0-109">Permission type</span></span>                        | <span data-ttu-id="d3ee0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3ee0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d3ee0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3ee0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3ee0-112">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3ee0-112">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="d3ee0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3ee0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3ee0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3ee0-114">Not supported.</span></span> |
| <span data-ttu-id="d3ee0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3ee0-115">Application</span></span>                            | <span data-ttu-id="d3ee0-116">Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3ee0-116">Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="d3ee0-117">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="d3ee0-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="d3ee0-118">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="d3ee0-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="d3ee0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3ee0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3ee0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d3ee0-120">Optional query parameters</span></span>

<span data-ttu-id="d3ee0-121">此操作不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d3ee0-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3ee0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3ee0-122">Request headers</span></span>

| <span data-ttu-id="d3ee0-123">名称</span><span class="sxs-lookup"><span data-stu-id="d3ee0-123">Name</span></span>      |<span data-ttu-id="d3ee0-124">说明</span><span class="sxs-lookup"><span data-stu-id="d3ee0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d3ee0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3ee0-125">Authorization</span></span> | <span data-ttu-id="d3ee0-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d3ee0-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3ee0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3ee0-127">Request body</span></span>

<span data-ttu-id="d3ee0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d3ee0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3ee0-129">响应</span><span class="sxs-lookup"><span data-stu-id="d3ee0-129">Response</span></span>

<span data-ttu-id="d3ee0-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatMessage](../resources/chatmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d3ee0-130">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3ee0-131">示例</span><span class="sxs-lookup"><span data-stu-id="d3ee0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3ee0-132">请求</span><span class="sxs-lookup"><span data-stu-id="d3ee0-132">Request</span></span>

<span data-ttu-id="d3ee0-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d3ee0-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3ee0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3ee0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/replies
```
# <a name="c"></a>[<span data-ttu-id="d3ee0-135">C#</span><span class="sxs-lookup"><span data-stu-id="d3ee0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3ee0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3ee0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3ee0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3ee0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3ee0-138">Java</span><span class="sxs-lookup"><span data-stu-id="d3ee0-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-replies-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3ee0-139">响应</span><span class="sxs-lookup"><span data-stu-id="d3ee0-139">Response</span></span>

<span data-ttu-id="d3ee0-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d3ee0-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d3ee0-141">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d3ee0-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d3ee0-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d3ee0-142">All the properties will be returned from an actual call.</span></span>

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


