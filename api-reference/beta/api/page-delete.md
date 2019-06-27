---
title: 删除页面
description: 删除 OneNote 页面。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: e1a28ea23e9988367e328eeaee03fec2e79ccaa6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265644"
---
# <a name="delete-page"></a><span data-ttu-id="f7ecb-103">删除页面</span><span class="sxs-lookup"><span data-stu-id="f7ecb-103">Delete page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7ecb-104">删除 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="f7ecb-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="f7ecb-105">权限</span><span class="sxs-lookup"><span data-stu-id="f7ecb-105">Permissions</span></span>
<span data-ttu-id="f7ecb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7ecb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7ecb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7ecb-108">Permission type</span></span>      | <span data-ttu-id="f7ecb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7ecb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7ecb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7ecb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7ecb-111">请注意, ReadWrite, All</span><span class="sxs-lookup"><span data-stu-id="f7ecb-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7ecb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7ecb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7ecb-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7ecb-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f7ecb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7ecb-114">Application</span></span> | <span data-ttu-id="f7ecb-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7ecb-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7ecb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7ecb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f7ecb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7ecb-117">Request headers</span></span>
| <span data-ttu-id="f7ecb-118">名称</span><span class="sxs-lookup"><span data-stu-id="f7ecb-118">Name</span></span>       | <span data-ttu-id="f7ecb-119">类型</span><span class="sxs-lookup"><span data-stu-id="f7ecb-119">Type</span></span> | <span data-ttu-id="f7ecb-120">说明</span><span class="sxs-lookup"><span data-stu-id="f7ecb-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f7ecb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7ecb-121">Authorization</span></span>  | <span data-ttu-id="f7ecb-122">string</span><span class="sxs-lookup"><span data-stu-id="f7ecb-122">string</span></span>  | <span data-ttu-id="f7ecb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7ecb-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f7ecb-125">响应</span><span class="sxs-lookup"><span data-stu-id="f7ecb-125">Response</span></span>

<span data-ttu-id="f7ecb-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f7ecb-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7ecb-128">示例</span><span class="sxs-lookup"><span data-stu-id="f7ecb-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7ecb-129">请求</span><span class="sxs-lookup"><span data-stu-id="f7ecb-129">Request</span></span>
<span data-ttu-id="f7ecb-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7ecb-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="f7ecb-131">响应</span><span class="sxs-lookup"><span data-stu-id="f7ecb-131">Response</span></span>
<span data-ttu-id="f7ecb-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f7ecb-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f7ecb-133">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f7ecb-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f7ecb-134">C#</span><span class="sxs-lookup"><span data-stu-id="f7ecb-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_page-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7ecb-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="f7ecb-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_page-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f7ecb-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="f7ecb-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_page-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/page-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/page-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/page-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
