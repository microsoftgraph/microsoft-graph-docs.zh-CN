---
title: 列出线程
description: 获取某个组的所有线程。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1c9cb896efc4124de87f0142eb624881c99be798
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517038"
---
# <a name="list-threads"></a><span data-ttu-id="ab4c6-103">列出线程</span><span class="sxs-lookup"><span data-stu-id="ab4c6-103">List threads</span></span>

<span data-ttu-id="ab4c6-104">命名空间： microsoft. graph 获取组的所有线程。</span><span class="sxs-lookup"><span data-stu-id="ab4c6-104">Namespace: microsoft.graph Get all the threads of a group.</span></span>

><span data-ttu-id="ab4c6-105">注意：还可以 [获取会话的所有线程](conversation-list-threads.md)。</span><span class="sxs-lookup"><span data-stu-id="ab4c6-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ab4c6-106">权限</span><span class="sxs-lookup"><span data-stu-id="ab4c6-106">Permissions</span></span>
<span data-ttu-id="ab4c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab4c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab4c6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab4c6-109">Permission type</span></span>      | <span data-ttu-id="ab4c6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab4c6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab4c6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab4c6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ab4c6-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab4c6-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab4c6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab4c6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab4c6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab4c6-114">Not supported.</span></span>    |
|<span data-ttu-id="ab4c6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab4c6-115">Application</span></span> | <span data-ttu-id="ab4c6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab4c6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab4c6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab4c6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab4c6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ab4c6-118">Optional query parameters</span></span>
<span data-ttu-id="ab4c6-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ab4c6-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab4c6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab4c6-120">Request headers</span></span>
| <span data-ttu-id="ab4c6-121">标头</span><span class="sxs-lookup"><span data-stu-id="ab4c6-121">Header</span></span>       | <span data-ttu-id="ab4c6-122">值</span><span class="sxs-lookup"><span data-stu-id="ab4c6-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab4c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab4c6-123">Authorization</span></span>  | <span data-ttu-id="ab4c6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ab4c6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab4c6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab4c6-126">Request body</span></span>
<span data-ttu-id="ab4c6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab4c6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab4c6-128">响应</span><span class="sxs-lookup"><span data-stu-id="ab4c6-128">Response</span></span>
<span data-ttu-id="ab4c6-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ConversationThread](../resources/conversationthread.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ab4c6-129">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab4c6-130">示例</span><span class="sxs-lookup"><span data-stu-id="ab4c6-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ab4c6-131">请求</span><span class="sxs-lookup"><span data-stu-id="ab4c6-131">Request</span></span>
<span data-ttu-id="ab4c6-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab4c6-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab4c6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab4c6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```
# <a name="c"></a>[<span data-ttu-id="ab4c6-134">C#</span><span class="sxs-lookup"><span data-stu-id="ab4c6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab4c6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab4c6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab4c6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab4c6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab4c6-137">Java</span><span class="sxs-lookup"><span data-stu-id="ab4c6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-threads-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ab4c6-138">响应</span><span class="sxs-lookup"><span data-stu-id="ab4c6-138">Response</span></span>
<span data-ttu-id="ab4c6-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ab4c6-139">The following is an example of the response.</span></span>
><span data-ttu-id="ab4c6-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ab4c6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "datetime-value",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
