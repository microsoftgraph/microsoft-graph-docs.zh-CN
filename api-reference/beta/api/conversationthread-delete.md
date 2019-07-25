---
title: 删除 conversationThread
description: 删除 conversationThread。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: e0fc12d6eb3dde6e925b2bfd63f58a4bea2c4692
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862952"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="abffc-103">删除 conversationThread</span><span class="sxs-lookup"><span data-stu-id="abffc-103">Delete conversationThread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abffc-104">删除 conversationThread。</span><span class="sxs-lookup"><span data-stu-id="abffc-104">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="abffc-105">权限</span><span class="sxs-lookup"><span data-stu-id="abffc-105">Permissions</span></span>
<span data-ttu-id="abffc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="abffc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abffc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="abffc-108">Permission type</span></span>      | <span data-ttu-id="abffc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="abffc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abffc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="abffc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="abffc-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abffc-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="abffc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="abffc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abffc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="abffc-113">Not supported.</span></span>    |
|<span data-ttu-id="abffc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="abffc-114">Application</span></span> | <span data-ttu-id="abffc-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abffc-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="abffc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="abffc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="abffc-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="abffc-117">Request headers</span></span>
| <span data-ttu-id="abffc-118">标头</span><span class="sxs-lookup"><span data-stu-id="abffc-118">Header</span></span>       | <span data-ttu-id="abffc-119">值</span><span class="sxs-lookup"><span data-stu-id="abffc-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="abffc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="abffc-120">Authorization</span></span>  | <span data-ttu-id="abffc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="abffc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="abffc-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="abffc-123">Request body</span></span>
<span data-ttu-id="abffc-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="abffc-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abffc-125">响应</span><span class="sxs-lookup"><span data-stu-id="abffc-125">Response</span></span>

<span data-ttu-id="abffc-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="abffc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abffc-128">示例</span><span class="sxs-lookup"><span data-stu-id="abffc-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="abffc-129">请求</span><span class="sxs-lookup"><span data-stu-id="abffc-129">Request</span></span>
<span data-ttu-id="abffc-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="abffc-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="abffc-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="abffc-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="abffc-132">C#</span><span class="sxs-lookup"><span data-stu-id="abffc-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="abffc-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="abffc-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="abffc-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="abffc-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="abffc-135">Java</span><span class="sxs-lookup"><span data-stu-id="abffc-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-conversationthread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="abffc-136">响应</span><span class="sxs-lookup"><span data-stu-id="abffc-136">Response</span></span>
<span data-ttu-id="abffc-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="abffc-137">Here is an example of the response.</span></span> 
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
