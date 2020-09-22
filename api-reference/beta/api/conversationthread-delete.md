---
title: 删除 conversationThread
description: 删除 conversationThread。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2e2692b17a0146826d38a033b4b04e6a1119248f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002695"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="cec91-103">删除 conversationThread</span><span class="sxs-lookup"><span data-stu-id="cec91-103">Delete conversationThread</span></span>

<span data-ttu-id="cec91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cec91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cec91-105">删除 conversationThread。</span><span class="sxs-lookup"><span data-stu-id="cec91-105">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="cec91-106">权限</span><span class="sxs-lookup"><span data-stu-id="cec91-106">Permissions</span></span>
<span data-ttu-id="cec91-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cec91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cec91-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cec91-109">Permission type</span></span>      | <span data-ttu-id="cec91-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cec91-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cec91-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cec91-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cec91-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cec91-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cec91-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cec91-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cec91-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cec91-114">Not supported.</span></span>    |
|<span data-ttu-id="cec91-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cec91-115">Application</span></span> | <span data-ttu-id="cec91-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cec91-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cec91-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cec91-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="cec91-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cec91-118">Request headers</span></span>
| <span data-ttu-id="cec91-119">标头</span><span class="sxs-lookup"><span data-stu-id="cec91-119">Header</span></span>       | <span data-ttu-id="cec91-120">值</span><span class="sxs-lookup"><span data-stu-id="cec91-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cec91-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cec91-121">Authorization</span></span>  | <span data-ttu-id="cec91-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cec91-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cec91-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="cec91-124">Request body</span></span>
<span data-ttu-id="cec91-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cec91-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cec91-126">响应</span><span class="sxs-lookup"><span data-stu-id="cec91-126">Response</span></span>

<span data-ttu-id="cec91-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cec91-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cec91-129">示例</span><span class="sxs-lookup"><span data-stu-id="cec91-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cec91-130">请求</span><span class="sxs-lookup"><span data-stu-id="cec91-130">Request</span></span>
<span data-ttu-id="cec91-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cec91-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cec91-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cec91-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
# <a name="c"></a>[<span data-ttu-id="cec91-133">C#</span><span class="sxs-lookup"><span data-stu-id="cec91-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cec91-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cec91-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cec91-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cec91-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cec91-136">响应</span><span class="sxs-lookup"><span data-stu-id="cec91-136">Response</span></span>
<span data-ttu-id="cec91-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cec91-137">Here is an example of the response.</span></span> 
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
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


