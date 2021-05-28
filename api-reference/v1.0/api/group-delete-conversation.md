---
title: 删除对话
description: 删除 conversation 对象。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 962216fbb34f63de654de877b2833befab95b739
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682605"
---
# <a name="delete-conversation"></a><span data-ttu-id="cfd0a-103">删除对话</span><span class="sxs-lookup"><span data-stu-id="cfd0a-103">Delete conversation</span></span>

<span data-ttu-id="cfd0a-104">命名空间：microsoft.graph 删除 [对话](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cfd0a-104">Namespace: microsoft.graph Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfd0a-105">权限</span><span class="sxs-lookup"><span data-stu-id="cfd0a-105">Permissions</span></span>
<span data-ttu-id="cfd0a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfd0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfd0a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfd0a-108">Permission type</span></span>      | <span data-ttu-id="cfd0a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cfd0a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfd0a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfd0a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cfd0a-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfd0a-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cfd0a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfd0a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfd0a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfd0a-113">Not supported.</span></span>    |
|<span data-ttu-id="cfd0a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfd0a-114">Application</span></span> | <span data-ttu-id="cfd0a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfd0a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfd0a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfd0a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cfd0a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfd0a-117">Request headers</span></span>
| <span data-ttu-id="cfd0a-118">名称</span><span class="sxs-lookup"><span data-stu-id="cfd0a-118">Name</span></span>       | <span data-ttu-id="cfd0a-119">类型</span><span class="sxs-lookup"><span data-stu-id="cfd0a-119">Type</span></span> | <span data-ttu-id="cfd0a-120">说明</span><span class="sxs-lookup"><span data-stu-id="cfd0a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cfd0a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfd0a-121">Authorization</span></span>  | <span data-ttu-id="cfd0a-122">string</span><span class="sxs-lookup"><span data-stu-id="cfd0a-122">string</span></span>  | <span data-ttu-id="cfd0a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cfd0a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfd0a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfd0a-125">Request body</span></span>
<span data-ttu-id="cfd0a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cfd0a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfd0a-127">响应</span><span class="sxs-lookup"><span data-stu-id="cfd0a-127">Response</span></span>
<span data-ttu-id="cfd0a-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cfd0a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfd0a-130">示例</span><span class="sxs-lookup"><span data-stu-id="cfd0a-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cfd0a-131">请求</span><span class="sxs-lookup"><span data-stu-id="cfd0a-131">Request</span></span>
<span data-ttu-id="cfd0a-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cfd0a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cfd0a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfd0a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="c"></a>[<span data-ttu-id="cfd0a-134">C#</span><span class="sxs-lookup"><span data-stu-id="cfd0a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfd0a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfd0a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfd0a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfd0a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfd0a-137">Java</span><span class="sxs-lookup"><span data-stu-id="cfd0a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cfd0a-138">响应</span><span class="sxs-lookup"><span data-stu-id="cfd0a-138">Response</span></span>
<span data-ttu-id="cfd0a-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cfd0a-139">The following is an example of the response.</span></span> 
><span data-ttu-id="cfd0a-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cfd0a-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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

