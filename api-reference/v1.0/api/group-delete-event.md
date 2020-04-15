---
title: 删除事件
description: 删除 event 对象。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6a88be728fa85c2380e032b49209c9440dc55912
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461425"
---
# <a name="delete-event"></a><span data-ttu-id="0d523-103">删除事件</span><span class="sxs-lookup"><span data-stu-id="0d523-103">Delete event</span></span>

<span data-ttu-id="0d523-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d523-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d523-105">删除 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0d523-105">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d523-106">权限</span><span class="sxs-lookup"><span data-stu-id="0d523-106">Permissions</span></span>
<span data-ttu-id="0d523-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d523-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d523-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d523-109">Permission type</span></span>      | <span data-ttu-id="0d523-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d523-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d523-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d523-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d523-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d523-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0d523-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d523-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d523-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d523-114">Not supported.</span></span>    |
|<span data-ttu-id="0d523-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d523-115">Application</span></span> | <span data-ttu-id="0d523-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d523-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d523-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d523-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0d523-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d523-118">Request headers</span></span>
| <span data-ttu-id="0d523-119">名称</span><span class="sxs-lookup"><span data-stu-id="0d523-119">Name</span></span>       | <span data-ttu-id="0d523-120">类型</span><span class="sxs-lookup"><span data-stu-id="0d523-120">Type</span></span> | <span data-ttu-id="0d523-121">说明</span><span class="sxs-lookup"><span data-stu-id="0d523-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0d523-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d523-122">Authorization</span></span>  | <span data-ttu-id="0d523-123">string</span><span class="sxs-lookup"><span data-stu-id="0d523-123">string</span></span>  | <span data-ttu-id="0d523-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0d523-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d523-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d523-126">Request body</span></span>
<span data-ttu-id="0d523-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0d523-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d523-128">响应</span><span class="sxs-lookup"><span data-stu-id="0d523-128">Response</span></span>
<span data-ttu-id="0d523-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0d523-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d523-131">示例</span><span class="sxs-lookup"><span data-stu-id="0d523-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0d523-132">请求</span><span class="sxs-lookup"><span data-stu-id="0d523-132">Request</span></span>
<span data-ttu-id="0d523-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0d523-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d523-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d523-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA=="],
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```
# <a name="c"></a>[<span data-ttu-id="0d523-135">C#</span><span class="sxs-lookup"><span data-stu-id="0d523-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d523-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d523-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d523-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d523-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d523-138">Java</span><span class="sxs-lookup"><span data-stu-id="0d523-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0d523-139">响应</span><span class="sxs-lookup"><span data-stu-id="0d523-139">Response</span></span>
<span data-ttu-id="0d523-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0d523-140">The following is an example of the response.</span></span> 
><span data-ttu-id="0d523-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0d523-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
