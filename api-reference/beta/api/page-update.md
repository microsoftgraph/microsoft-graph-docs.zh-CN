---
title: 更新页面
description: 更新 OneNote 页面的内容。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 4f3b8d219249b578f1876b1b30df7f3c7d2487b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004590"
---
# <a name="update-page"></a><span data-ttu-id="5e51c-103">更新页面</span><span class="sxs-lookup"><span data-stu-id="5e51c-103">Update page</span></span>

<span data-ttu-id="5e51c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e51c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e51c-105">更新 OneNote 页面的内容。</span><span class="sxs-lookup"><span data-stu-id="5e51c-105">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="5e51c-106">权限</span><span class="sxs-lookup"><span data-stu-id="5e51c-106">Permissions</span></span>
<span data-ttu-id="5e51c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e51c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e51c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e51c-109">Permission type</span></span>      | <span data-ttu-id="5e51c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e51c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e51c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e51c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5e51c-112">请注意，ReadWrite，All</span><span class="sxs-lookup"><span data-stu-id="5e51c-112">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5e51c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e51c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e51c-114">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e51c-114">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5e51c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e51c-115">Application</span></span> | <span data-ttu-id="5e51c-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e51c-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e51c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e51c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="5e51c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e51c-118">Request headers</span></span>
| <span data-ttu-id="5e51c-119">名称</span><span class="sxs-lookup"><span data-stu-id="5e51c-119">Name</span></span>       | <span data-ttu-id="5e51c-120">类型</span><span class="sxs-lookup"><span data-stu-id="5e51c-120">Type</span></span> | <span data-ttu-id="5e51c-121">说明</span><span class="sxs-lookup"><span data-stu-id="5e51c-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5e51c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e51c-122">Authorization</span></span>  | <span data-ttu-id="5e51c-123">string</span><span class="sxs-lookup"><span data-stu-id="5e51c-123">string</span></span>  | <span data-ttu-id="5e51c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e51c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e51c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e51c-126">Content-Type</span></span> | <span data-ttu-id="5e51c-127">string</span><span class="sxs-lookup"><span data-stu-id="5e51c-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5e51c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e51c-128">Request body</span></span>
<span data-ttu-id="5e51c-129">在请求正文中，提供 [patchContentCommand](../resources/patchcontentcommand.md) 对象的数组，这些对象代表页面的更改。</span><span class="sxs-lookup"><span data-stu-id="5e51c-129">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="5e51c-130">有关详细信息和示例，请参阅 [更新 OneNote 页面内容](/graph/onenote-update-page)。</span><span class="sxs-lookup"><span data-stu-id="5e51c-130">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="5e51c-131">响应</span><span class="sxs-lookup"><span data-stu-id="5e51c-131">Response</span></span>

<span data-ttu-id="5e51c-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5e51c-132">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="5e51c-133">PATCH 请求未返回任何 JSON 数据。</span><span class="sxs-lookup"><span data-stu-id="5e51c-133">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="5e51c-134">示例</span><span class="sxs-lookup"><span data-stu-id="5e51c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e51c-135">请求</span><span class="sxs-lookup"><span data-stu-id="5e51c-135">Request</span></span>
<span data-ttu-id="5e51c-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e51c-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e51c-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e51c-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
# <a name="c"></a>[<span data-ttu-id="5e51c-138">C#</span><span class="sxs-lookup"><span data-stu-id="5e51c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e51c-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e51c-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e51c-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e51c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5e51c-141">响应</span><span class="sxs-lookup"><span data-stu-id="5e51c-141">Response</span></span>
<span data-ttu-id="5e51c-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5e51c-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


