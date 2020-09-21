---
title: 删除 conversationThread
description: 删除 conversationThread。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a3b6207681eb67ea38b26cff8e8b5a14ff70de0a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010022"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="a89f4-103">删除 conversationThread</span><span class="sxs-lookup"><span data-stu-id="a89f4-103">Delete conversationThread</span></span>

<span data-ttu-id="a89f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a89f4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a89f4-105">删除 conversationThread。</span><span class="sxs-lookup"><span data-stu-id="a89f4-105">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="a89f4-106">权限</span><span class="sxs-lookup"><span data-stu-id="a89f4-106">Permissions</span></span>
<span data-ttu-id="a89f4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a89f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a89f4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a89f4-109">Permission type</span></span>      | <span data-ttu-id="a89f4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a89f4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a89f4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a89f4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a89f4-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a89f4-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a89f4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a89f4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a89f4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a89f4-114">Not supported.</span></span>    |
|<span data-ttu-id="a89f4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a89f4-115">Application</span></span> | <span data-ttu-id="a89f4-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a89f4-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a89f4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a89f4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="a89f4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a89f4-118">Request headers</span></span>
| <span data-ttu-id="a89f4-119">标头</span><span class="sxs-lookup"><span data-stu-id="a89f4-119">Header</span></span>       | <span data-ttu-id="a89f4-120">值</span><span class="sxs-lookup"><span data-stu-id="a89f4-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a89f4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a89f4-121">Authorization</span></span>  | <span data-ttu-id="a89f4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a89f4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a89f4-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="a89f4-124">Request body</span></span>
<span data-ttu-id="a89f4-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a89f4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a89f4-126">响应</span><span class="sxs-lookup"><span data-stu-id="a89f4-126">Response</span></span>

<span data-ttu-id="a89f4-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a89f4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a89f4-129">示例</span><span class="sxs-lookup"><span data-stu-id="a89f4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a89f4-130">请求</span><span class="sxs-lookup"><span data-stu-id="a89f4-130">Request</span></span>
<span data-ttu-id="a89f4-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a89f4-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a89f4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a89f4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
# <a name="c"></a>[<span data-ttu-id="a89f4-133">C#</span><span class="sxs-lookup"><span data-stu-id="a89f4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a89f4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a89f4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a89f4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a89f4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a89f4-136">Java</span><span class="sxs-lookup"><span data-stu-id="a89f4-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-conversationthread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a89f4-137">响应</span><span class="sxs-lookup"><span data-stu-id="a89f4-137">Response</span></span>
<span data-ttu-id="a89f4-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a89f4-138">Here is an example of the response.</span></span> 
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
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

