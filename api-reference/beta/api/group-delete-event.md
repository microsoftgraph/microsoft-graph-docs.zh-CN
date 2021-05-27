---
title: 删除事件
description: 删除 event 对象。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c86fe5e188c5a5ce025b56a336922552d8098625
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681853"
---
# <a name="delete-event"></a><span data-ttu-id="94cba-103">删除事件</span><span class="sxs-lookup"><span data-stu-id="94cba-103">Delete event</span></span>

<span data-ttu-id="94cba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94cba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94cba-105">删除 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94cba-105">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="94cba-106">权限</span><span class="sxs-lookup"><span data-stu-id="94cba-106">Permissions</span></span>
<span data-ttu-id="94cba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94cba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94cba-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="94cba-109">Permission type</span></span>      | <span data-ttu-id="94cba-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94cba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94cba-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94cba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="94cba-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94cba-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="94cba-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94cba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94cba-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="94cba-114">Not supported.</span></span>    |
|<span data-ttu-id="94cba-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="94cba-115">Application</span></span> | <span data-ttu-id="94cba-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="94cba-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94cba-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94cba-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="94cba-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="94cba-118">Request headers</span></span>
| <span data-ttu-id="94cba-119">名称</span><span class="sxs-lookup"><span data-stu-id="94cba-119">Name</span></span>       | <span data-ttu-id="94cba-120">类型</span><span class="sxs-lookup"><span data-stu-id="94cba-120">Type</span></span> | <span data-ttu-id="94cba-121">说明</span><span class="sxs-lookup"><span data-stu-id="94cba-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="94cba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94cba-122">Authorization</span></span>  | <span data-ttu-id="94cba-123">string</span><span class="sxs-lookup"><span data-stu-id="94cba-123">string</span></span>  | <span data-ttu-id="94cba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94cba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94cba-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="94cba-126">Request body</span></span>
<span data-ttu-id="94cba-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94cba-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94cba-128">响应</span><span class="sxs-lookup"><span data-stu-id="94cba-128">Response</span></span>
<span data-ttu-id="94cba-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="94cba-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94cba-131">示例</span><span class="sxs-lookup"><span data-stu-id="94cba-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="94cba-132">请求</span><span class="sxs-lookup"><span data-stu-id="94cba-132">Request</span></span>
<span data-ttu-id="94cba-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="94cba-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94cba-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="94cba-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```
# <a name="c"></a>[<span data-ttu-id="94cba-135">C#</span><span class="sxs-lookup"><span data-stu-id="94cba-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94cba-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94cba-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94cba-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94cba-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94cba-138">Java</span><span class="sxs-lookup"><span data-stu-id="94cba-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94cba-139">响应</span><span class="sxs-lookup"><span data-stu-id="94cba-139">Response</span></span>
<span data-ttu-id="94cba-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="94cba-140">The following is an example of the response.</span></span> 
><span data-ttu-id="94cba-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="94cba-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


