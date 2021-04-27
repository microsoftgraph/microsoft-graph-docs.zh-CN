---
title: 删除对话
description: 删除 conversation 对象。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5da2c54e86cb6d59c8220be89f05681914fd56b7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042021"
---
# <a name="delete-conversation"></a><span data-ttu-id="36ba2-103">删除对话</span><span class="sxs-lookup"><span data-stu-id="36ba2-103">Delete conversation</span></span>

<span data-ttu-id="36ba2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36ba2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36ba2-105">删除 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36ba2-105">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="36ba2-106">权限</span><span class="sxs-lookup"><span data-stu-id="36ba2-106">Permissions</span></span>
<span data-ttu-id="36ba2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36ba2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36ba2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="36ba2-109">Permission type</span></span>      | <span data-ttu-id="36ba2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36ba2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36ba2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36ba2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="36ba2-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36ba2-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="36ba2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36ba2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36ba2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="36ba2-114">Not supported.</span></span>    |
|<span data-ttu-id="36ba2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="36ba2-115">Application</span></span> | <span data-ttu-id="36ba2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="36ba2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36ba2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36ba2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="36ba2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="36ba2-118">Request headers</span></span>
| <span data-ttu-id="36ba2-119">名称</span><span class="sxs-lookup"><span data-stu-id="36ba2-119">Name</span></span>       | <span data-ttu-id="36ba2-120">类型</span><span class="sxs-lookup"><span data-stu-id="36ba2-120">Type</span></span> | <span data-ttu-id="36ba2-121">说明</span><span class="sxs-lookup"><span data-stu-id="36ba2-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="36ba2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36ba2-122">Authorization</span></span>  | <span data-ttu-id="36ba2-123">string</span><span class="sxs-lookup"><span data-stu-id="36ba2-123">string</span></span>  | <span data-ttu-id="36ba2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36ba2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36ba2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="36ba2-126">Request body</span></span>
<span data-ttu-id="36ba2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36ba2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36ba2-128">响应</span><span class="sxs-lookup"><span data-stu-id="36ba2-128">Response</span></span>
<span data-ttu-id="36ba2-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="36ba2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36ba2-131">示例</span><span class="sxs-lookup"><span data-stu-id="36ba2-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="36ba2-132">请求</span><span class="sxs-lookup"><span data-stu-id="36ba2-132">Request</span></span>
<span data-ttu-id="36ba2-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="36ba2-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="36ba2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="36ba2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="c"></a>[<span data-ttu-id="36ba2-135">C#</span><span class="sxs-lookup"><span data-stu-id="36ba2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36ba2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36ba2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36ba2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36ba2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36ba2-138">Java</span><span class="sxs-lookup"><span data-stu-id="36ba2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36ba2-139">响应</span><span class="sxs-lookup"><span data-stu-id="36ba2-139">Response</span></span>
<span data-ttu-id="36ba2-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="36ba2-140">The following is an example of the response.</span></span> 
><span data-ttu-id="36ba2-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="36ba2-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


