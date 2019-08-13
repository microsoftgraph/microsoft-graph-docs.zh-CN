---
title: 更新页面
description: 更新 OneNote 页面的内容。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 95022c80220349176289fd2d0797571cee45c5bd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349598"
---
# <a name="update-page"></a><span data-ttu-id="e8846-103">更新页面</span><span class="sxs-lookup"><span data-stu-id="e8846-103">Update page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8846-104">更新 OneNote 页面的内容。</span><span class="sxs-lookup"><span data-stu-id="e8846-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="e8846-105">权限</span><span class="sxs-lookup"><span data-stu-id="e8846-105">Permissions</span></span>
<span data-ttu-id="e8846-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8846-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8846-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8846-108">Permission type</span></span>      | <span data-ttu-id="e8846-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8846-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8846-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8846-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8846-111">请注意, ReadWrite, All</span><span class="sxs-lookup"><span data-stu-id="e8846-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8846-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8846-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8846-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8846-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e8846-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8846-114">Application</span></span> | <span data-ttu-id="e8846-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8846-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8846-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8846-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="e8846-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8846-117">Request headers</span></span>
| <span data-ttu-id="e8846-118">名称</span><span class="sxs-lookup"><span data-stu-id="e8846-118">Name</span></span>       | <span data-ttu-id="e8846-119">类型</span><span class="sxs-lookup"><span data-stu-id="e8846-119">Type</span></span> | <span data-ttu-id="e8846-120">说明</span><span class="sxs-lookup"><span data-stu-id="e8846-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e8846-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8846-121">Authorization</span></span>  | <span data-ttu-id="e8846-122">string</span><span class="sxs-lookup"><span data-stu-id="e8846-122">string</span></span>  | <span data-ttu-id="e8846-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8846-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8846-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8846-125">Content-Type</span></span> | <span data-ttu-id="e8846-126">string</span><span class="sxs-lookup"><span data-stu-id="e8846-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e8846-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8846-127">Request body</span></span>
<span data-ttu-id="e8846-128">在请求正文中, 提供[patchContentCommand](../resources/patchcontentcommand.md)对象的数组, 这些对象代表页面的更改。</span><span class="sxs-lookup"><span data-stu-id="e8846-128">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="e8846-129">有关详细信息和示例, 请参阅[更新 OneNote 页面内容](/graph/onenote-update-page)。</span><span class="sxs-lookup"><span data-stu-id="e8846-129">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="e8846-130">响应</span><span class="sxs-lookup"><span data-stu-id="e8846-130">Response</span></span>

<span data-ttu-id="e8846-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e8846-131">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="e8846-132">PATCH 请求未返回任何 JSON 数据。</span><span class="sxs-lookup"><span data-stu-id="e8846-132">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="e8846-133">示例</span><span class="sxs-lookup"><span data-stu-id="e8846-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8846-134">请求</span><span class="sxs-lookup"><span data-stu-id="e8846-134">Request</span></span>
<span data-ttu-id="e8846-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8846-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e8846-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e8846-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e8846-137">C#</span><span class="sxs-lookup"><span data-stu-id="e8846-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8846-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8846-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e8846-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="e8846-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e8846-140">Java</span><span class="sxs-lookup"><span data-stu-id="e8846-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-page-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e8846-141">响应</span><span class="sxs-lookup"><span data-stu-id="e8846-141">Response</span></span>
<span data-ttu-id="e8846-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e8846-142">Here is an example of the response.</span></span> 
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
