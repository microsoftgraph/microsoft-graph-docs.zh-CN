---
title: 更新页面
description: 更新 OneNote 页面的内容。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: fc1e43542728b9590ed4983cdf32e8de277a0467
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402008"
---
# <a name="update-page"></a><span data-ttu-id="1a15d-103">更新页面</span><span class="sxs-lookup"><span data-stu-id="1a15d-103">Update page</span></span>

<span data-ttu-id="1a15d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a15d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a15d-105">更新 OneNote 页面的内容。</span><span class="sxs-lookup"><span data-stu-id="1a15d-105">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a15d-106">权限</span><span class="sxs-lookup"><span data-stu-id="1a15d-106">Permissions</span></span>
<span data-ttu-id="1a15d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a15d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a15d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a15d-109">Permission type</span></span>      | <span data-ttu-id="1a15d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a15d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a15d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a15d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1a15d-112">请注意，ReadWrite，All</span><span class="sxs-lookup"><span data-stu-id="1a15d-112">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a15d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a15d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a15d-114">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a15d-114">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1a15d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a15d-115">Application</span></span> | <span data-ttu-id="1a15d-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a15d-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a15d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a15d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="1a15d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a15d-118">Request headers</span></span>
| <span data-ttu-id="1a15d-119">名称</span><span class="sxs-lookup"><span data-stu-id="1a15d-119">Name</span></span>       | <span data-ttu-id="1a15d-120">类型</span><span class="sxs-lookup"><span data-stu-id="1a15d-120">Type</span></span> | <span data-ttu-id="1a15d-121">说明</span><span class="sxs-lookup"><span data-stu-id="1a15d-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1a15d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a15d-122">Authorization</span></span>  | <span data-ttu-id="1a15d-123">string</span><span class="sxs-lookup"><span data-stu-id="1a15d-123">string</span></span>  | <span data-ttu-id="1a15d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a15d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a15d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a15d-126">Content-Type</span></span> | <span data-ttu-id="1a15d-127">string</span><span class="sxs-lookup"><span data-stu-id="1a15d-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1a15d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a15d-128">Request body</span></span>
<span data-ttu-id="1a15d-129">在请求正文中，提供 [patchContentCommand](../resources/patchcontentcommand.md) 对象的数组，这些对象代表页面的更改。</span><span class="sxs-lookup"><span data-stu-id="1a15d-129">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="1a15d-130">有关详细信息和示例，请参阅 <a href="/graph/onenote-update-page">更新 OneNote 页面</a>。</span><span class="sxs-lookup"><span data-stu-id="1a15d-130">For more information and examples, see <a href="/graph/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="1a15d-131">响应</span><span class="sxs-lookup"><span data-stu-id="1a15d-131">Response</span></span>

<span data-ttu-id="1a15d-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1a15d-132">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="1a15d-133">PATCH 请求未返回任何 JSON 数据。</span><span class="sxs-lookup"><span data-stu-id="1a15d-133">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="1a15d-134">示例</span><span class="sxs-lookup"><span data-stu-id="1a15d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a15d-135">请求</span><span class="sxs-lookup"><span data-stu-id="1a15d-135">Request</span></span>
<span data-ttu-id="1a15d-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a15d-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a15d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a15d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
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
# <a name="c"></a>[<span data-ttu-id="1a15d-138">C#</span><span class="sxs-lookup"><span data-stu-id="1a15d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a15d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a15d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a15d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a15d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a15d-141">Java</span><span class="sxs-lookup"><span data-stu-id="1a15d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-page-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1a15d-142">响应</span><span class="sxs-lookup"><span data-stu-id="1a15d-142">Response</span></span>
<span data-ttu-id="1a15d-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1a15d-143">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->