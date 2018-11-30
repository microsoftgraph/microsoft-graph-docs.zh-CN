---
title: 更新页面
description: 更新 OneNote 页面的内容。
ms.openlocfilehash: 862271da69985b7386f5025d630227b6222cd64a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046637"
---
# <a name="update-page"></a><span data-ttu-id="4837c-103">更新页面</span><span class="sxs-lookup"><span data-stu-id="4837c-103">Update page</span></span>

> <span data-ttu-id="4837c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4837c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4837c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4837c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4837c-106">更新 OneNote 页面的内容。</span><span class="sxs-lookup"><span data-stu-id="4837c-106">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="4837c-107">权限</span><span class="sxs-lookup"><span data-stu-id="4837c-107">Permissions</span></span>
<span data-ttu-id="4837c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4837c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4837c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4837c-110">Permission type</span></span>      | <span data-ttu-id="4837c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4837c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4837c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4837c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4837c-113">Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4837c-113">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4837c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4837c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4837c-115">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4837c-115">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4837c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4837c-116">Application</span></span> | <span data-ttu-id="4837c-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4837c-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4837c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4837c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="4837c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4837c-119">Request headers</span></span>
| <span data-ttu-id="4837c-120">名称</span><span class="sxs-lookup"><span data-stu-id="4837c-120">Name</span></span>       | <span data-ttu-id="4837c-121">类型</span><span class="sxs-lookup"><span data-stu-id="4837c-121">Type</span></span> | <span data-ttu-id="4837c-122">说明</span><span class="sxs-lookup"><span data-stu-id="4837c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4837c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4837c-123">Authorization</span></span>  | <span data-ttu-id="4837c-124">string</span><span class="sxs-lookup"><span data-stu-id="4837c-124">string</span></span>  | <span data-ttu-id="4837c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4837c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4837c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4837c-127">Content-Type</span></span> | <span data-ttu-id="4837c-128">string</span><span class="sxs-lookup"><span data-stu-id="4837c-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4837c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4837c-129">Request body</span></span>
<span data-ttu-id="4837c-130">在请求正文中，提供[patchContentCommand](../resources/patchcontentcommand.md)对象表示的更改 ' 页上的数组。</span><span class="sxs-lookup"><span data-stu-id="4837c-130">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="4837c-131">有关详细信息和示例，请参阅[更新 OneNote 页面内容](/graph/onenote-update-page)。</span><span class="sxs-lookup"><span data-stu-id="4837c-131">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="4837c-132">响应</span><span class="sxs-lookup"><span data-stu-id="4837c-132">Response</span></span>

<span data-ttu-id="4837c-p105">如果成功，此方法返回 `204 No Content` 响应代码。PATCH 请求未返回任何 JSON 数据。</span><span class="sxs-lookup"><span data-stu-id="4837c-p105">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="4837c-135">示例</span><span class="sxs-lookup"><span data-stu-id="4837c-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4837c-136">请求</span><span class="sxs-lookup"><span data-stu-id="4837c-136">Request</span></span>
<span data-ttu-id="4837c-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4837c-137">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="4837c-138">响应</span><span class="sxs-lookup"><span data-stu-id="4837c-138">Response</span></span>
<span data-ttu-id="4837c-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4837c-139">Here is an example of the response.</span></span> 
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
  "tocPath": ""
}-->
