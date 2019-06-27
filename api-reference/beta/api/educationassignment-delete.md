---
title: 删除 educationAssignment
description: 删除现有工作分配。 只有课堂中的教师才能删除工作分配。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 408e5495a816de2832a3ac18d40110cd79c1b979
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259939"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="0941b-104">删除 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="0941b-104">Delete educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0941b-105">删除现有工作分配。</span><span class="sxs-lookup"><span data-stu-id="0941b-105">Delete an existing assignment.</span></span> <span data-ttu-id="0941b-106">只有课堂中的教师才能删除工作分配。</span><span class="sxs-lookup"><span data-stu-id="0941b-106">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="0941b-107">权限</span><span class="sxs-lookup"><span data-stu-id="0941b-107">Permissions</span></span>

<span data-ttu-id="0941b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0941b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0941b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0941b-110">Permission type</span></span>                        | <span data-ttu-id="0941b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0941b-111">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="0941b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0941b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0941b-113">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="0941b-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="0941b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0941b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0941b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0941b-115">Not Supported.</span></span>                                          |
| <span data-ttu-id="0941b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0941b-116">Application</span></span>                            | <span data-ttu-id="0941b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0941b-117">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="0941b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0941b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0941b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0941b-119">Request headers</span></span>

| <span data-ttu-id="0941b-120">标头</span><span class="sxs-lookup"><span data-stu-id="0941b-120">Header</span></span>        | <span data-ttu-id="0941b-121">值</span><span class="sxs-lookup"><span data-stu-id="0941b-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="0941b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0941b-122">Authorization</span></span> | <span data-ttu-id="0941b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0941b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0941b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0941b-125">Request body</span></span>

<span data-ttu-id="0941b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0941b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0941b-127">响应</span><span class="sxs-lookup"><span data-stu-id="0941b-127">Response</span></span>

<span data-ttu-id="0941b-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0941b-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0941b-130">示例</span><span class="sxs-lookup"><span data-stu-id="0941b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0941b-131">请求</span><span class="sxs-lookup"><span data-stu-id="0941b-131">Request</span></span>

<span data-ttu-id="0941b-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0941b-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a><span data-ttu-id="0941b-133">响应</span><span class="sxs-lookup"><span data-stu-id="0941b-133">Response</span></span>
<span data-ttu-id="0941b-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0941b-134">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0941b-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="0941b-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0941b-136">C#</span><span class="sxs-lookup"><span data-stu-id="0941b-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0941b-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="0941b-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationassignment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0941b-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="0941b-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_educationassignment-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
