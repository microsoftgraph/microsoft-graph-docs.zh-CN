---
title: 删除 educationSchool
description: 删除学校。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 61db44ba60fb7ede58f2568b1afb2b0b8deddc7d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259652"
---
# <a name="delete-educationschool"></a><span data-ttu-id="43f4f-103">删除 educationSchool</span><span class="sxs-lookup"><span data-stu-id="43f4f-103">Delete educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43f4f-104">删除学校。</span><span class="sxs-lookup"><span data-stu-id="43f4f-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="43f4f-105">权限</span><span class="sxs-lookup"><span data-stu-id="43f4f-105">Permissions</span></span>
<span data-ttu-id="43f4f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43f4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43f4f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="43f4f-108">Permission type</span></span>      | <span data-ttu-id="43f4f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43f4f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43f4f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43f4f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="43f4f-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="43f4f-111">Not supported.</span></span>  |
|<span data-ttu-id="43f4f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43f4f-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="43f4f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="43f4f-113">Not supported.</span></span>  |
|<span data-ttu-id="43f4f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="43f4f-114">Application</span></span> | <span data-ttu-id="43f4f-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43f4f-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="43f4f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43f4f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="43f4f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="43f4f-117">Request headers</span></span>
| <span data-ttu-id="43f4f-118">标头</span><span class="sxs-lookup"><span data-stu-id="43f4f-118">Header</span></span>       | <span data-ttu-id="43f4f-119">值</span><span class="sxs-lookup"><span data-stu-id="43f4f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="43f4f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="43f4f-120">Authorization</span></span>  | <span data-ttu-id="43f4f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="43f4f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="43f4f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="43f4f-123">Request body</span></span>
<span data-ttu-id="43f4f-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="43f4f-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="43f4f-125">响应</span><span class="sxs-lookup"><span data-stu-id="43f4f-125">Response</span></span>
<span data-ttu-id="43f4f-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="43f4f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43f4f-128">示例</span><span class="sxs-lookup"><span data-stu-id="43f4f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="43f4f-129">请求</span><span class="sxs-lookup"><span data-stu-id="43f4f-129">Request</span></span>
<span data-ttu-id="43f4f-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="43f4f-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10002
```
##### <a name="response"></a><span data-ttu-id="43f4f-131">响应</span><span class="sxs-lookup"><span data-stu-id="43f4f-131">Response</span></span>
<span data-ttu-id="43f4f-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="43f4f-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="43f4f-133">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="43f4f-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="43f4f-134">C#</span><span class="sxs-lookup"><span data-stu-id="43f4f-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationschool-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="43f4f-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="43f4f-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationschool-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="43f4f-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="43f4f-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_educationschool-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationschool-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationschool-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationschool-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
