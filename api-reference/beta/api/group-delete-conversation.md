---
title: 删除对话
description: 删除 conversation 对象。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8017e9151b15e61a61945ab1200c88d0fc92d563
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681863"
---
# <a name="delete-conversation"></a><span data-ttu-id="63945-103">删除对话</span><span class="sxs-lookup"><span data-stu-id="63945-103">Delete conversation</span></span>

<span data-ttu-id="63945-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63945-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63945-105">删除 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63945-105">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="63945-106">权限</span><span class="sxs-lookup"><span data-stu-id="63945-106">Permissions</span></span>
<span data-ttu-id="63945-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63945-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63945-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="63945-109">Permission type</span></span>      | <span data-ttu-id="63945-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63945-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63945-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63945-111">Delegated (work or school account)</span></span> | <span data-ttu-id="63945-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63945-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="63945-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63945-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63945-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="63945-114">Not supported.</span></span>    |
|<span data-ttu-id="63945-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="63945-115">Application</span></span> | <span data-ttu-id="63945-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="63945-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63945-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63945-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="63945-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="63945-118">Request headers</span></span>
| <span data-ttu-id="63945-119">名称</span><span class="sxs-lookup"><span data-stu-id="63945-119">Name</span></span>       | <span data-ttu-id="63945-120">类型</span><span class="sxs-lookup"><span data-stu-id="63945-120">Type</span></span> | <span data-ttu-id="63945-121">说明</span><span class="sxs-lookup"><span data-stu-id="63945-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="63945-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="63945-122">Authorization</span></span>  | <span data-ttu-id="63945-123">string</span><span class="sxs-lookup"><span data-stu-id="63945-123">string</span></span>  | <span data-ttu-id="63945-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63945-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63945-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="63945-126">Request body</span></span>
<span data-ttu-id="63945-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63945-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63945-128">响应</span><span class="sxs-lookup"><span data-stu-id="63945-128">Response</span></span>
<span data-ttu-id="63945-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="63945-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63945-131">示例</span><span class="sxs-lookup"><span data-stu-id="63945-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="63945-132">请求</span><span class="sxs-lookup"><span data-stu-id="63945-132">Request</span></span>
<span data-ttu-id="63945-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="63945-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63945-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="63945-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="c"></a>[<span data-ttu-id="63945-135">C#</span><span class="sxs-lookup"><span data-stu-id="63945-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63945-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63945-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63945-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63945-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63945-138">Java</span><span class="sxs-lookup"><span data-stu-id="63945-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="63945-139">响应</span><span class="sxs-lookup"><span data-stu-id="63945-139">Response</span></span>
<span data-ttu-id="63945-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63945-140">The following is an example of the response.</span></span> 
><span data-ttu-id="63945-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="63945-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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


