---
title: 更新页面
description: 更新 OneNote 页面的内容。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 9de057a4162a77b7c48729ed7e756cc94ba3cb38
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276655"
---
# <a name="update-page"></a><span data-ttu-id="eb556-103">更新页面</span><span class="sxs-lookup"><span data-stu-id="eb556-103">Update page</span></span>

<span data-ttu-id="eb556-104">更新 OneNote 页面的内容。</span><span class="sxs-lookup"><span data-stu-id="eb556-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="eb556-105">权限</span><span class="sxs-lookup"><span data-stu-id="eb556-105">Permissions</span></span>
<span data-ttu-id="eb556-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb556-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb556-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb556-108">Permission type</span></span>      | <span data-ttu-id="eb556-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb556-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb556-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb556-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eb556-111">请注意, ReadWrite, All</span><span class="sxs-lookup"><span data-stu-id="eb556-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb556-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb556-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb556-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb556-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="eb556-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb556-114">Application</span></span> | <span data-ttu-id="eb556-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb556-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb556-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb556-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="eb556-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb556-117">Request headers</span></span>
| <span data-ttu-id="eb556-118">名称</span><span class="sxs-lookup"><span data-stu-id="eb556-118">Name</span></span>       | <span data-ttu-id="eb556-119">类型</span><span class="sxs-lookup"><span data-stu-id="eb556-119">Type</span></span> | <span data-ttu-id="eb556-120">说明</span><span class="sxs-lookup"><span data-stu-id="eb556-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="eb556-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb556-121">Authorization</span></span>  | <span data-ttu-id="eb556-122">string</span><span class="sxs-lookup"><span data-stu-id="eb556-122">string</span></span>  | <span data-ttu-id="eb556-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb556-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb556-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb556-125">Content-Type</span></span> | <span data-ttu-id="eb556-126">string</span><span class="sxs-lookup"><span data-stu-id="eb556-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="eb556-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb556-127">Request body</span></span>
<span data-ttu-id="eb556-128">在请求正文中, 提供[patchContentCommand](../resources/patchcontentcommand.md)对象的数组, 这些对象代表页面的更改。</span><span class="sxs-lookup"><span data-stu-id="eb556-128">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="eb556-129">有关详细信息和示例, 请参阅<a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">更新 OneNote 页面</a>。</span><span class="sxs-lookup"><span data-stu-id="eb556-129">For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="eb556-130">响应</span><span class="sxs-lookup"><span data-stu-id="eb556-130">Response</span></span>

<span data-ttu-id="eb556-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="eb556-131">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="eb556-132">PATCH 请求未返回任何 JSON 数据。</span><span class="sxs-lookup"><span data-stu-id="eb556-132">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="eb556-133">示例</span><span class="sxs-lookup"><span data-stu-id="eb556-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb556-134">请求</span><span class="sxs-lookup"><span data-stu-id="eb556-134">Request</span></span>
<span data-ttu-id="eb556-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb556-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="eb556-136">响应</span><span class="sxs-lookup"><span data-stu-id="eb556-136">Response</span></span>
<span data-ttu-id="eb556-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="eb556-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="eb556-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="eb556-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eb556-139">C#</span><span class="sxs-lookup"><span data-stu-id="eb556-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_page-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb556-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="eb556-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_page-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="eb556-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="eb556-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_page-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/page-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/page-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/page-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
