---
title: 删除 educationCategory
description: 删除现有类别。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7cb8704d0ab48ae60b31675b9df75f3ad5070c1d
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750057"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="21aaf-103">删除 educationCategory</span><span class="sxs-lookup"><span data-stu-id="21aaf-103">Delete educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21aaf-104">删除现有类别。</span><span class="sxs-lookup"><span data-stu-id="21aaf-104">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="21aaf-105">权限</span><span class="sxs-lookup"><span data-stu-id="21aaf-105">Permissions</span></span>

<span data-ttu-id="21aaf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21aaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="21aaf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="21aaf-108">Permission type</span></span>                        | <span data-ttu-id="21aaf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="21aaf-109">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="21aaf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21aaf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="21aaf-111">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="21aaf-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="21aaf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21aaf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21aaf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="21aaf-113">Not Supported.</span></span>                                          |
| <span data-ttu-id="21aaf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="21aaf-114">Application</span></span>                            | <span data-ttu-id="21aaf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="21aaf-115">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="21aaf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21aaf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="21aaf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="21aaf-117">Request headers</span></span>

| <span data-ttu-id="21aaf-118">标头</span><span class="sxs-lookup"><span data-stu-id="21aaf-118">Header</span></span>        | <span data-ttu-id="21aaf-119">值</span><span class="sxs-lookup"><span data-stu-id="21aaf-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="21aaf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="21aaf-120">Authorization</span></span> | <span data-ttu-id="21aaf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="21aaf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21aaf-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="21aaf-123">Request body</span></span>

<span data-ttu-id="21aaf-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="21aaf-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21aaf-125">响应</span><span class="sxs-lookup"><span data-stu-id="21aaf-125">Response</span></span>

<span data-ttu-id="21aaf-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="21aaf-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21aaf-128">示例</span><span class="sxs-lookup"><span data-stu-id="21aaf-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="21aaf-129">请求</span><span class="sxs-lookup"><span data-stu-id="21aaf-129">Request</span></span>

<span data-ttu-id="21aaf-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="21aaf-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```

### <a name="response"></a><span data-ttu-id="21aaf-131">响应</span><span class="sxs-lookup"><span data-stu-id="21aaf-131">Response</span></span>

<span data-ttu-id="21aaf-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="21aaf-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

#### <a name="sdk-sample-code"></a><span data-ttu-id="21aaf-133">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="21aaf-133">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="21aaf-134">C#</span><span class="sxs-lookup"><span data-stu-id="21aaf-134">C#</span></span>](#tab/cs)

[!INCLUDE [sample-code](../includes/delete_educationassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21aaf-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="21aaf-135">Javascript</span></span>](#tab/javascript)

[!INCLUDE [sample-code](../includes/delete_educationassignment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationcategory-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationcategory-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
