---
title: 列出对话
description: 检索此组中的会话列表。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: fb0088df0f89f52fe68bd55330d0ca71f168e9d6
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682577"
---
# <a name="list-conversations"></a><span data-ttu-id="3b9b1-103">列出对话</span><span class="sxs-lookup"><span data-stu-id="3b9b1-103">List conversations</span></span>

<span data-ttu-id="3b9b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b9b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b9b1-105">检索此组中的[对话](../resources/conversation.md)列表。</span><span class="sxs-lookup"><span data-stu-id="3b9b1-105">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b9b1-106">权限</span><span class="sxs-lookup"><span data-stu-id="3b9b1-106">Permissions</span></span>
<span data-ttu-id="3b9b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b9b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b9b1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b9b1-109">Permission type</span></span>      | <span data-ttu-id="3b9b1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b9b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b9b1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b9b1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3b9b1-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b9b1-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b9b1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b9b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b9b1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b9b1-114">Not supported.</span></span>    |
|<span data-ttu-id="3b9b1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b9b1-115">Application</span></span> | <span data-ttu-id="3b9b1-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b9b1-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b9b1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b9b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b9b1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3b9b1-118">Optional query parameters</span></span>
<span data-ttu-id="3b9b1-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3b9b1-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b9b1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b9b1-120">Request headers</span></span>
| <span data-ttu-id="3b9b1-121">标头</span><span class="sxs-lookup"><span data-stu-id="3b9b1-121">Header</span></span>       | <span data-ttu-id="3b9b1-122">值</span><span class="sxs-lookup"><span data-stu-id="3b9b1-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b9b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b9b1-123">Authorization</span></span>  | <span data-ttu-id="3b9b1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3b9b1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b9b1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b9b1-126">Request body</span></span>
<span data-ttu-id="3b9b1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3b9b1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b9b1-128">响应</span><span class="sxs-lookup"><span data-stu-id="3b9b1-128">Response</span></span>
<span data-ttu-id="3b9b1-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Conversation](../resources/conversation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3b9b1-129">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b9b1-130">示例</span><span class="sxs-lookup"><span data-stu-id="3b9b1-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3b9b1-131">请求</span><span class="sxs-lookup"><span data-stu-id="3b9b1-131">Request</span></span>
<span data-ttu-id="3b9b1-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3b9b1-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3b9b1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b9b1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
# <a name="c"></a>[<span data-ttu-id="3b9b1-134">C#</span><span class="sxs-lookup"><span data-stu-id="3b9b1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b9b1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b9b1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b9b1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b9b1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b9b1-137">Java</span><span class="sxs-lookup"><span data-stu-id="3b9b1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3b9b1-138">响应</span><span class="sxs-lookup"><span data-stu-id="3b9b1-138">Response</span></span>
<span data-ttu-id="3b9b1-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3b9b1-139">The following is an example of the response.</span></span>
><span data-ttu-id="3b9b1-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3b9b1-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

