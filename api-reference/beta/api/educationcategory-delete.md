---
title: 删除 educationCategory
description: 删除现有类别。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a1a74d0755dae8c83a62a7acf92cd34ef0245d1a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002490"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="42b2e-103">删除 educationCategory</span><span class="sxs-lookup"><span data-stu-id="42b2e-103">Delete educationCategory</span></span>

<span data-ttu-id="42b2e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42b2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42b2e-105">删除现有类别。</span><span class="sxs-lookup"><span data-stu-id="42b2e-105">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="42b2e-106">权限</span><span class="sxs-lookup"><span data-stu-id="42b2e-106">Permissions</span></span>

<span data-ttu-id="42b2e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42b2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42b2e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="42b2e-109">Permission type</span></span>                        | <span data-ttu-id="42b2e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42b2e-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="42b2e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42b2e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="42b2e-112">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="42b2e-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="42b2e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42b2e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42b2e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="42b2e-114">Not Supported.</span></span>                                          |
| <span data-ttu-id="42b2e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="42b2e-115">Application</span></span>                            | <span data-ttu-id="42b2e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="42b2e-116">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="42b2e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42b2e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="42b2e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="42b2e-118">Request headers</span></span>

| <span data-ttu-id="42b2e-119">标头</span><span class="sxs-lookup"><span data-stu-id="42b2e-119">Header</span></span>        | <span data-ttu-id="42b2e-120">值</span><span class="sxs-lookup"><span data-stu-id="42b2e-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="42b2e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="42b2e-121">Authorization</span></span> | <span data-ttu-id="42b2e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="42b2e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42b2e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="42b2e-124">Request body</span></span>

<span data-ttu-id="42b2e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="42b2e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42b2e-126">响应</span><span class="sxs-lookup"><span data-stu-id="42b2e-126">Response</span></span>

<span data-ttu-id="42b2e-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="42b2e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42b2e-129">示例</span><span class="sxs-lookup"><span data-stu-id="42b2e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="42b2e-130">请求</span><span class="sxs-lookup"><span data-stu-id="42b2e-130">Request</span></span>

<span data-ttu-id="42b2e-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="42b2e-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="42b2e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="42b2e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
# <a name="c"></a>[<span data-ttu-id="42b2e-133">C#</span><span class="sxs-lookup"><span data-stu-id="42b2e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42b2e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42b2e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42b2e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42b2e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42b2e-136">响应</span><span class="sxs-lookup"><span data-stu-id="42b2e-136">Response</span></span>

<span data-ttu-id="42b2e-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="42b2e-137">The following is an example of the response.</span></span> 

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


