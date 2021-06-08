---
title: 更新页面
description: 更新页面OneNote内容。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: f6f0fb24188beb64502d2ef91c389f66677465fe
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785135"
---
# <a name="update-page"></a><span data-ttu-id="1b89a-103">更新页面</span><span class="sxs-lookup"><span data-stu-id="1b89a-103">Update page</span></span>

<span data-ttu-id="1b89a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b89a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b89a-105">更新页面OneNote内容。</span><span class="sxs-lookup"><span data-stu-id="1b89a-105">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="1b89a-106">权限</span><span class="sxs-lookup"><span data-stu-id="1b89a-106">Permissions</span></span>
<span data-ttu-id="1b89a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b89a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b89a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b89a-109">Permission type</span></span>      | <span data-ttu-id="1b89a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b89a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b89a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b89a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1b89a-112">Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b89a-112">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b89a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b89a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b89a-114">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b89a-114">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1b89a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b89a-115">Application</span></span> | <span data-ttu-id="1b89a-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b89a-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b89a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b89a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="1b89a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b89a-118">Request headers</span></span>
| <span data-ttu-id="1b89a-119">名称</span><span class="sxs-lookup"><span data-stu-id="1b89a-119">Name</span></span>       | <span data-ttu-id="1b89a-120">类型</span><span class="sxs-lookup"><span data-stu-id="1b89a-120">Type</span></span> | <span data-ttu-id="1b89a-121">说明</span><span class="sxs-lookup"><span data-stu-id="1b89a-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1b89a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b89a-122">Authorization</span></span>  | <span data-ttu-id="1b89a-123">string</span><span class="sxs-lookup"><span data-stu-id="1b89a-123">string</span></span>  | <span data-ttu-id="1b89a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1b89a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1b89a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b89a-126">Content-Type</span></span> | <span data-ttu-id="1b89a-127">string</span><span class="sxs-lookup"><span data-stu-id="1b89a-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1b89a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b89a-128">Request body</span></span>
<span data-ttu-id="1b89a-129">在请求正文中，提供一个 [patchContentCommand](../resources/patchcontentcommand.md) 对象数组，这些对象代表对页面的更改。</span><span class="sxs-lookup"><span data-stu-id="1b89a-129">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="1b89a-130">有关详细信息和示例，请参阅更新OneNote[页面内容](/graph/onenote-update-page)。</span><span class="sxs-lookup"><span data-stu-id="1b89a-130">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="1b89a-131">响应</span><span class="sxs-lookup"><span data-stu-id="1b89a-131">Response</span></span>

<span data-ttu-id="1b89a-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1b89a-132">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="1b89a-133">PATCH 请求未返回任何 JSON 数据。</span><span class="sxs-lookup"><span data-stu-id="1b89a-133">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="1b89a-134">示例</span><span class="sxs-lookup"><span data-stu-id="1b89a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b89a-135">请求</span><span class="sxs-lookup"><span data-stu-id="1b89a-135">Request</span></span>
<span data-ttu-id="1b89a-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1b89a-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b89a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b89a-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1b89a-138">C#</span><span class="sxs-lookup"><span data-stu-id="1b89a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b89a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b89a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b89a-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b89a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1b89a-141">响应</span><span class="sxs-lookup"><span data-stu-id="1b89a-141">Response</span></span>
<span data-ttu-id="1b89a-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1b89a-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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


