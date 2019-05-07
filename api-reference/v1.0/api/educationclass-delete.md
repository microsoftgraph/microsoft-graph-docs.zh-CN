---
title: 删除 educationClass
description: 删除课程。 课程也是通用组，因此删除课程时也会删除组。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 1e12201386ab3e14155f04f4408c364334e0b0d5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616065"
---
# <a name="delete-educationclass"></a><span data-ttu-id="11ee0-104">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="11ee0-104">Delete educationClass</span></span>

<span data-ttu-id="11ee0-105">删除课程。</span><span class="sxs-lookup"><span data-stu-id="11ee0-105">Delete a class.</span></span> <span data-ttu-id="11ee0-106">课程也是通用组，因此删除课程时也会删除组。</span><span class="sxs-lookup"><span data-stu-id="11ee0-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="11ee0-107">权限</span><span class="sxs-lookup"><span data-stu-id="11ee0-107">Permissions</span></span>
<span data-ttu-id="11ee0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11ee0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11ee0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="11ee0-110">Permission type</span></span>      | <span data-ttu-id="11ee0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="11ee0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11ee0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11ee0-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="11ee0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="11ee0-113">Not supported.</span></span>  |
|<span data-ttu-id="11ee0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11ee0-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="11ee0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="11ee0-115">Not supported.</span></span>  |
|<span data-ttu-id="11ee0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="11ee0-116">Application</span></span> | <span data-ttu-id="11ee0-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11ee0-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="11ee0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11ee0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="11ee0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="11ee0-119">Request headers</span></span>
| <span data-ttu-id="11ee0-120">标头</span><span class="sxs-lookup"><span data-stu-id="11ee0-120">Header</span></span>       | <span data-ttu-id="11ee0-121">值</span><span class="sxs-lookup"><span data-stu-id="11ee0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="11ee0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="11ee0-122">Authorization</span></span>  | <span data-ttu-id="11ee0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="11ee0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="11ee0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="11ee0-125">Request body</span></span>
<span data-ttu-id="11ee0-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="11ee0-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="11ee0-127">响应</span><span class="sxs-lookup"><span data-stu-id="11ee0-127">Response</span></span>
<span data-ttu-id="11ee0-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="11ee0-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11ee0-130">示例</span><span class="sxs-lookup"><span data-stu-id="11ee0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11ee0-131">请求</span><span class="sxs-lookup"><span data-stu-id="11ee0-131">Request</span></span>
<span data-ttu-id="11ee0-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="11ee0-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="11ee0-133">响应</span><span class="sxs-lookup"><span data-stu-id="11ee0-133">Response</span></span>
<span data-ttu-id="11ee0-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="11ee0-134">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="11ee0-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="11ee0-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="11ee0-136">语言</span><span class="sxs-lookup"><span data-stu-id="11ee0-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationclass-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11ee0-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="11ee0-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationclass-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/educationclass-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationclass-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
