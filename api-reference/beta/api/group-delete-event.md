---
title: 删除事件
description: 删除 event 对象。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3b1478076c9d176794d285d9997bc21b8271b658
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440699"
---
# <a name="delete-event"></a><span data-ttu-id="b0a6a-103">删除事件</span><span class="sxs-lookup"><span data-stu-id="b0a6a-103">Delete event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0a6a-104">删除 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b0a6a-104">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0a6a-105">权限</span><span class="sxs-lookup"><span data-stu-id="b0a6a-105">Permissions</span></span>
<span data-ttu-id="b0a6a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0a6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0a6a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0a6a-108">Permission type</span></span>      | <span data-ttu-id="b0a6a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0a6a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0a6a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0a6a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b0a6a-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0a6a-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b0a6a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0a6a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0a6a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0a6a-113">Not supported.</span></span>    |
|<span data-ttu-id="b0a6a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0a6a-114">Application</span></span> | <span data-ttu-id="b0a6a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0a6a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0a6a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0a6a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b0a6a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0a6a-117">Request headers</span></span>
| <span data-ttu-id="b0a6a-118">名称</span><span class="sxs-lookup"><span data-stu-id="b0a6a-118">Name</span></span>       | <span data-ttu-id="b0a6a-119">类型</span><span class="sxs-lookup"><span data-stu-id="b0a6a-119">Type</span></span> | <span data-ttu-id="b0a6a-120">说明</span><span class="sxs-lookup"><span data-stu-id="b0a6a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b0a6a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0a6a-121">Authorization</span></span>  | <span data-ttu-id="b0a6a-122">string</span><span class="sxs-lookup"><span data-stu-id="b0a6a-122">string</span></span>  | <span data-ttu-id="b0a6a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b0a6a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0a6a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0a6a-125">Request body</span></span>
<span data-ttu-id="b0a6a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b0a6a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0a6a-127">响应</span><span class="sxs-lookup"><span data-stu-id="b0a6a-127">Response</span></span>
<span data-ttu-id="b0a6a-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b0a6a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0a6a-130">示例</span><span class="sxs-lookup"><span data-stu-id="b0a6a-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b0a6a-131">请求</span><span class="sxs-lookup"><span data-stu-id="b0a6a-131">Request</span></span>
<span data-ttu-id="b0a6a-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b0a6a-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b0a6a-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b0a6a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0a6a-134">C#</span><span class="sxs-lookup"><span data-stu-id="b0a6a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0a6a-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0a6a-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0a6a-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="b0a6a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b0a6a-137">响应</span><span class="sxs-lookup"><span data-stu-id="b0a6a-137">Response</span></span>
<span data-ttu-id="b0a6a-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b0a6a-138">The following is an example of the response.</span></span> 
><span data-ttu-id="b0a6a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b0a6a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
