---
title: 删除对话
description: 删除对话。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e231236b99d838759a6132e133ff24745b052856
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518215"
---
# <a name="delete-conversation"></a><span data-ttu-id="2d324-103">删除对话</span><span class="sxs-lookup"><span data-stu-id="2d324-103">Delete conversation</span></span>

<span data-ttu-id="2d324-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d324-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d324-105">删除对话。</span><span class="sxs-lookup"><span data-stu-id="2d324-105">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="2d324-106">权限</span><span class="sxs-lookup"><span data-stu-id="2d324-106">Permissions</span></span>
<span data-ttu-id="2d324-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d324-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d324-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d324-109">Permission type</span></span>      | <span data-ttu-id="2d324-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d324-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d324-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d324-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2d324-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d324-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2d324-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d324-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d324-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d324-114">Not supported.</span></span>    |
|<span data-ttu-id="2d324-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d324-115">Application</span></span> | <span data-ttu-id="2d324-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d324-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d324-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d324-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2d324-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d324-118">Request headers</span></span>
| <span data-ttu-id="2d324-119">标头</span><span class="sxs-lookup"><span data-stu-id="2d324-119">Header</span></span>       | <span data-ttu-id="2d324-120">值</span><span class="sxs-lookup"><span data-stu-id="2d324-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2d324-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d324-121">Authorization</span></span>  | <span data-ttu-id="2d324-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d324-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2d324-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d324-124">Request body</span></span>
<span data-ttu-id="2d324-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2d324-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d324-126">响应</span><span class="sxs-lookup"><span data-stu-id="2d324-126">Response</span></span>

<span data-ttu-id="2d324-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2d324-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d324-129">示例</span><span class="sxs-lookup"><span data-stu-id="2d324-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d324-130">请求</span><span class="sxs-lookup"><span data-stu-id="2d324-130">Request</span></span>
<span data-ttu-id="2d324-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d324-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2d324-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d324-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
# <a name="c"></a>[<span data-ttu-id="2d324-133">C#</span><span class="sxs-lookup"><span data-stu-id="2d324-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d324-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d324-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d324-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d324-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d324-136">Java</span><span class="sxs-lookup"><span data-stu-id="2d324-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2d324-137">响应</span><span class="sxs-lookup"><span data-stu-id="2d324-137">Response</span></span>
<span data-ttu-id="2d324-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2d324-138">Here is an example of the response.</span></span> 
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
