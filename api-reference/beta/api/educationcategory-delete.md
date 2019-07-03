---
title: 删除 educationCategory
description: 删除现有类别。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5230f7d4d2091222893b18ba4a5f2857d4b2ad3d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436100"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="56649-103">删除 educationCategory</span><span class="sxs-lookup"><span data-stu-id="56649-103">Delete educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56649-104">删除现有类别。</span><span class="sxs-lookup"><span data-stu-id="56649-104">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="56649-105">权限</span><span class="sxs-lookup"><span data-stu-id="56649-105">Permissions</span></span>

<span data-ttu-id="56649-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56649-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56649-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="56649-108">Permission type</span></span>                        | <span data-ttu-id="56649-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56649-109">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="56649-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56649-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="56649-111">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="56649-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="56649-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56649-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56649-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="56649-113">Not Supported.</span></span>                                          |
| <span data-ttu-id="56649-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="56649-114">Application</span></span>                            | <span data-ttu-id="56649-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="56649-115">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="56649-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56649-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="56649-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="56649-117">Request headers</span></span>

| <span data-ttu-id="56649-118">标头</span><span class="sxs-lookup"><span data-stu-id="56649-118">Header</span></span>        | <span data-ttu-id="56649-119">值</span><span class="sxs-lookup"><span data-stu-id="56649-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="56649-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="56649-120">Authorization</span></span> | <span data-ttu-id="56649-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="56649-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56649-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="56649-123">Request body</span></span>

<span data-ttu-id="56649-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56649-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56649-125">响应</span><span class="sxs-lookup"><span data-stu-id="56649-125">Response</span></span>

<span data-ttu-id="56649-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="56649-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56649-128">示例</span><span class="sxs-lookup"><span data-stu-id="56649-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="56649-129">请求</span><span class="sxs-lookup"><span data-stu-id="56649-129">Request</span></span>

<span data-ttu-id="56649-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="56649-130">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="56649-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="56649-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="56649-132">C#</span><span class="sxs-lookup"><span data-stu-id="56649-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56649-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="56649-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="56649-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="56649-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="56649-135">响应</span><span class="sxs-lookup"><span data-stu-id="56649-135">Response</span></span>

<span data-ttu-id="56649-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="56649-136">The following is an example of the response.</span></span> 

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
  "description": "Delete educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
