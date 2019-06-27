---
title: 删除 educationClass
description: 删除课程。 课程也是通用组，因此删除课程时也会删除组。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 28cd82de286594efd70363041184bb86e3c04a2b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271734"
---
# <a name="delete-educationclass"></a><span data-ttu-id="f861c-104">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="f861c-104">Delete educationClass</span></span>

<span data-ttu-id="f861c-105">删除课程。</span><span class="sxs-lookup"><span data-stu-id="f861c-105">Delete a class.</span></span> <span data-ttu-id="f861c-106">课程也是通用组，因此删除课程时也会删除组。</span><span class="sxs-lookup"><span data-stu-id="f861c-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="f861c-107">权限</span><span class="sxs-lookup"><span data-stu-id="f861c-107">Permissions</span></span>
<span data-ttu-id="f861c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f861c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f861c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f861c-110">Permission type</span></span>      | <span data-ttu-id="f861c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f861c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f861c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f861c-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="f861c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f861c-113">Not supported.</span></span>  |
|<span data-ttu-id="f861c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f861c-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f861c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f861c-115">Not supported.</span></span>  |
|<span data-ttu-id="f861c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f861c-116">Application</span></span> | <span data-ttu-id="f861c-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f861c-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f861c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f861c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="f861c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f861c-119">Request headers</span></span>
| <span data-ttu-id="f861c-120">标头</span><span class="sxs-lookup"><span data-stu-id="f861c-120">Header</span></span>       | <span data-ttu-id="f861c-121">值</span><span class="sxs-lookup"><span data-stu-id="f861c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f861c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f861c-122">Authorization</span></span>  | <span data-ttu-id="f861c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f861c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f861c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f861c-125">Request body</span></span>
<span data-ttu-id="f861c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f861c-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f861c-127">响应</span><span class="sxs-lookup"><span data-stu-id="f861c-127">Response</span></span>
<span data-ttu-id="f861c-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f861c-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f861c-130">示例</span><span class="sxs-lookup"><span data-stu-id="f861c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f861c-131">请求</span><span class="sxs-lookup"><span data-stu-id="f861c-131">Request</span></span>
<span data-ttu-id="f861c-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f861c-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="f861c-133">响应</span><span class="sxs-lookup"><span data-stu-id="f861c-133">Response</span></span>
<span data-ttu-id="f861c-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f861c-134">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f861c-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f861c-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f861c-136">C#</span><span class="sxs-lookup"><span data-stu-id="f861c-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationclass-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f861c-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="f861c-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationclass-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f861c-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="f861c-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_educationclass-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationclass-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/educationclass-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationclass-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
