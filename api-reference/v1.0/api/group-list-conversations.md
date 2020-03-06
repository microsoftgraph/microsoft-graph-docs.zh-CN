---
title: 列出对话
description: 检索此组中的会话列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 80b33bbb6f97f1c3cc820d46be21f3cea71365e8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517094"
---
# <a name="list-conversations"></a><span data-ttu-id="53301-103">列出对话</span><span class="sxs-lookup"><span data-stu-id="53301-103">List conversations</span></span>

<span data-ttu-id="53301-104">命名空间： microsoft. graph 检索此组中的[对话](../resources/conversation.md)列表。</span><span class="sxs-lookup"><span data-stu-id="53301-104">Namespace: microsoft.graph Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="53301-105">权限</span><span class="sxs-lookup"><span data-stu-id="53301-105">Permissions</span></span>
<span data-ttu-id="53301-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53301-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53301-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="53301-108">Permission type</span></span>      | <span data-ttu-id="53301-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53301-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53301-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53301-110">Delegated (work or school account)</span></span> | <span data-ttu-id="53301-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53301-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="53301-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53301-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53301-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="53301-113">Not supported.</span></span>    |
|<span data-ttu-id="53301-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="53301-114">Application</span></span> | <span data-ttu-id="53301-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="53301-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53301-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53301-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53301-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="53301-117">Optional query parameters</span></span>
<span data-ttu-id="53301-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="53301-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53301-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="53301-119">Request headers</span></span>
| <span data-ttu-id="53301-120">标头</span><span class="sxs-lookup"><span data-stu-id="53301-120">Header</span></span>       | <span data-ttu-id="53301-121">值</span><span class="sxs-lookup"><span data-stu-id="53301-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="53301-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53301-122">Authorization</span></span>  | <span data-ttu-id="53301-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53301-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53301-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="53301-125">Request body</span></span>
<span data-ttu-id="53301-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53301-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53301-127">响应</span><span class="sxs-lookup"><span data-stu-id="53301-127">Response</span></span>
<span data-ttu-id="53301-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Conversation](../resources/conversation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="53301-128">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53301-129">示例</span><span class="sxs-lookup"><span data-stu-id="53301-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="53301-130">请求</span><span class="sxs-lookup"><span data-stu-id="53301-130">Request</span></span>
<span data-ttu-id="53301-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53301-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53301-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="53301-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
# <a name="c"></a>[<span data-ttu-id="53301-133">C#</span><span class="sxs-lookup"><span data-stu-id="53301-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53301-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53301-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53301-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53301-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53301-136">Java</span><span class="sxs-lookup"><span data-stu-id="53301-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="53301-137">响应</span><span class="sxs-lookup"><span data-stu-id="53301-137">Response</span></span>
<span data-ttu-id="53301-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="53301-138">The following is an example of the response.</span></span>
><span data-ttu-id="53301-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="53301-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
