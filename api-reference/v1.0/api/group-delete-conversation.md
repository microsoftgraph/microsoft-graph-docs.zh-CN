---
title: 删除对话
description: 删除 conversation 对象。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 055066d04a46cc8e0358a86f78e7298c53470566
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856524"
---
# <a name="delete-conversation"></a><span data-ttu-id="502d7-103">删除对话</span><span class="sxs-lookup"><span data-stu-id="502d7-103">Delete conversation</span></span>
<span data-ttu-id="502d7-104">删除 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="502d7-104">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="502d7-105">权限</span><span class="sxs-lookup"><span data-stu-id="502d7-105">Permissions</span></span>
<span data-ttu-id="502d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="502d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="502d7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="502d7-108">Permission type</span></span>      | <span data-ttu-id="502d7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="502d7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="502d7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="502d7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="502d7-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="502d7-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="502d7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="502d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="502d7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="502d7-113">Not supported.</span></span>    |
|<span data-ttu-id="502d7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="502d7-114">Application</span></span> | <span data-ttu-id="502d7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="502d7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="502d7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="502d7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="502d7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="502d7-117">Request headers</span></span>
| <span data-ttu-id="502d7-118">名称</span><span class="sxs-lookup"><span data-stu-id="502d7-118">Name</span></span>       | <span data-ttu-id="502d7-119">类型</span><span class="sxs-lookup"><span data-stu-id="502d7-119">Type</span></span> | <span data-ttu-id="502d7-120">说明</span><span class="sxs-lookup"><span data-stu-id="502d7-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="502d7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="502d7-121">Authorization</span></span>  | <span data-ttu-id="502d7-122">string</span><span class="sxs-lookup"><span data-stu-id="502d7-122">string</span></span>  | <span data-ttu-id="502d7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="502d7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="502d7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="502d7-125">Request body</span></span>
<span data-ttu-id="502d7-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="502d7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="502d7-127">响应</span><span class="sxs-lookup"><span data-stu-id="502d7-127">Response</span></span>
<span data-ttu-id="502d7-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="502d7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="502d7-130">示例</span><span class="sxs-lookup"><span data-stu-id="502d7-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="502d7-131">请求</span><span class="sxs-lookup"><span data-stu-id="502d7-131">Request</span></span>
<span data-ttu-id="502d7-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="502d7-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="502d7-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="502d7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="502d7-134">C#</span><span class="sxs-lookup"><span data-stu-id="502d7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="502d7-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="502d7-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="502d7-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="502d7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="502d7-137">Java</span><span class="sxs-lookup"><span data-stu-id="502d7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="502d7-138">响应</span><span class="sxs-lookup"><span data-stu-id="502d7-138">Response</span></span>
<span data-ttu-id="502d7-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="502d7-139">The following is an example of the response.</span></span> 
><span data-ttu-id="502d7-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="502d7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
