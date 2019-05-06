---
title: 删除 educationAssignment
description: 删除现有工作分配。 只有课堂中的教师才能删除工作分配。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 22c5e7c2795377eaeba9e8bcacc0c188ed0995ef
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33588064"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="c4dd6-104">删除 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="c4dd6-104">Delete educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4dd6-105">删除现有工作分配。</span><span class="sxs-lookup"><span data-stu-id="c4dd6-105">Delete an existing assignment.</span></span> <span data-ttu-id="c4dd6-106">只有课堂中的教师才能删除工作分配。</span><span class="sxs-lookup"><span data-stu-id="c4dd6-106">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4dd6-107">权限</span><span class="sxs-lookup"><span data-stu-id="c4dd6-107">Permissions</span></span>
<span data-ttu-id="c4dd6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4dd6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4dd6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4dd6-110">Permission type</span></span>      | <span data-ttu-id="c4dd6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4dd6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4dd6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4dd6-112">Delegated (work or school account)</span></span>| <span data-ttu-id="c4dd6-113">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="c4dd6-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="c4dd6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4dd6-114">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="c4dd6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4dd6-115">Not Supported.</span></span> |
|<span data-ttu-id="c4dd6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4dd6-116">Application</span></span> | <span data-ttu-id="c4dd6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4dd6-117">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="c4dd6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4dd6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignments/<id>
```
## <a name="request-headers"></a><span data-ttu-id="c4dd6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4dd6-119">Request headers</span></span>
| <span data-ttu-id="c4dd6-120">标头</span><span class="sxs-lookup"><span data-stu-id="c4dd6-120">Header</span></span>       | <span data-ttu-id="c4dd6-121">值</span><span class="sxs-lookup"><span data-stu-id="c4dd6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c4dd6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4dd6-122">Authorization</span></span>  | <span data-ttu-id="c4dd6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4dd6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c4dd6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4dd6-125">Request body</span></span>
<span data-ttu-id="c4dd6-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c4dd6-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c4dd6-127">响应</span><span class="sxs-lookup"><span data-stu-id="c4dd6-127">Response</span></span>
<span data-ttu-id="c4dd6-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c4dd6-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4dd6-130">示例</span><span class="sxs-lookup"><span data-stu-id="c4dd6-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="c4dd6-131">请求</span><span class="sxs-lookup"><span data-stu-id="c4dd6-131">Request</span></span>
<span data-ttu-id="c4dd6-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c4dd6-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a><span data-ttu-id="c4dd6-133">响应</span><span class="sxs-lookup"><span data-stu-id="c4dd6-133">Response</span></span>
<span data-ttu-id="c4dd6-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c4dd6-134">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c4dd6-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c4dd6-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c4dd6-136">语言</span><span class="sxs-lookup"><span data-stu-id="c4dd6-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4dd6-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="c4dd6-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationassignment-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
