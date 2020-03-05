---
title: 删除页面
description: 删除 OneNote 页面。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: e58c3c5763b0ce40932f235640c7fbf193945b5f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456017"
---
# <a name="delete-page"></a><span data-ttu-id="11f0b-103">删除页面</span><span class="sxs-lookup"><span data-stu-id="11f0b-103">Delete page</span></span>

<span data-ttu-id="11f0b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="11f0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11f0b-105">删除 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="11f0b-105">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="11f0b-106">权限</span><span class="sxs-lookup"><span data-stu-id="11f0b-106">Permissions</span></span>
<span data-ttu-id="11f0b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11f0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11f0b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="11f0b-109">Permission type</span></span>      | <span data-ttu-id="11f0b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="11f0b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11f0b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11f0b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="11f0b-112">请注意，ReadWrite，All</span><span class="sxs-lookup"><span data-stu-id="11f0b-112">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="11f0b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11f0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11f0b-114">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11f0b-114">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="11f0b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="11f0b-115">Application</span></span> | <span data-ttu-id="11f0b-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11f0b-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11f0b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11f0b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="11f0b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="11f0b-118">Request headers</span></span>
| <span data-ttu-id="11f0b-119">名称</span><span class="sxs-lookup"><span data-stu-id="11f0b-119">Name</span></span>       | <span data-ttu-id="11f0b-120">类型</span><span class="sxs-lookup"><span data-stu-id="11f0b-120">Type</span></span> | <span data-ttu-id="11f0b-121">说明</span><span class="sxs-lookup"><span data-stu-id="11f0b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="11f0b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="11f0b-122">Authorization</span></span>  | <span data-ttu-id="11f0b-123">string</span><span class="sxs-lookup"><span data-stu-id="11f0b-123">string</span></span>  | <span data-ttu-id="11f0b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="11f0b-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="11f0b-126">响应</span><span class="sxs-lookup"><span data-stu-id="11f0b-126">Response</span></span>

<span data-ttu-id="11f0b-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="11f0b-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11f0b-129">示例</span><span class="sxs-lookup"><span data-stu-id="11f0b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11f0b-130">请求</span><span class="sxs-lookup"><span data-stu-id="11f0b-130">Request</span></span>
<span data-ttu-id="11f0b-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="11f0b-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11f0b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="11f0b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
# <a name="c"></a>[<span data-ttu-id="11f0b-133">C#</span><span class="sxs-lookup"><span data-stu-id="11f0b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11f0b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11f0b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11f0b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11f0b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="11f0b-136">响应</span><span class="sxs-lookup"><span data-stu-id="11f0b-136">Response</span></span>
<span data-ttu-id="11f0b-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="11f0b-137">Here is an example of the response.</span></span>
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
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
