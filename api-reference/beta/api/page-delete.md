---
title: 删除页面
description: 删除 OneNote 页面。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: a1e10d1f2c5fac96efcd9dbc3b2909c900981594
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453871"
---
# <a name="delete-page"></a><span data-ttu-id="81560-103">删除页面</span><span class="sxs-lookup"><span data-stu-id="81560-103">Delete page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81560-104">删除 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="81560-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="81560-105">权限</span><span class="sxs-lookup"><span data-stu-id="81560-105">Permissions</span></span>
<span data-ttu-id="81560-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81560-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81560-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="81560-108">Permission type</span></span>      | <span data-ttu-id="81560-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="81560-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81560-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81560-110">Delegated (work or school account)</span></span> | <span data-ttu-id="81560-111">请注意, ReadWrite, All</span><span class="sxs-lookup"><span data-stu-id="81560-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="81560-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81560-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81560-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81560-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="81560-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="81560-114">Application</span></span> | <span data-ttu-id="81560-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81560-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81560-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81560-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="81560-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="81560-117">Request headers</span></span>
| <span data-ttu-id="81560-118">名称</span><span class="sxs-lookup"><span data-stu-id="81560-118">Name</span></span>       | <span data-ttu-id="81560-119">类型</span><span class="sxs-lookup"><span data-stu-id="81560-119">Type</span></span> | <span data-ttu-id="81560-120">说明</span><span class="sxs-lookup"><span data-stu-id="81560-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="81560-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="81560-121">Authorization</span></span>  | <span data-ttu-id="81560-122">string</span><span class="sxs-lookup"><span data-stu-id="81560-122">string</span></span>  | <span data-ttu-id="81560-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="81560-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="81560-125">响应</span><span class="sxs-lookup"><span data-stu-id="81560-125">Response</span></span>

<span data-ttu-id="81560-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="81560-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81560-128">示例</span><span class="sxs-lookup"><span data-stu-id="81560-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81560-129">请求</span><span class="sxs-lookup"><span data-stu-id="81560-129">Request</span></span>
<span data-ttu-id="81560-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="81560-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="81560-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="81560-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="81560-132">C#</span><span class="sxs-lookup"><span data-stu-id="81560-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81560-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="81560-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="81560-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="81560-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="81560-135">响应</span><span class="sxs-lookup"><span data-stu-id="81560-135">Response</span></span>
<span data-ttu-id="81560-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="81560-136">Here is an example of the response.</span></span>
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
