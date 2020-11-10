---
title: 删除 educationAssignment
description: 删除现有工作分配。 只有课堂中的教师才能删除工作分配。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3e85d23fc4ef128a3c1231f51a8a037036b0a3d7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966589"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="bb328-104">删除 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="bb328-104">Delete educationAssignment</span></span>

<span data-ttu-id="bb328-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb328-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb328-106">删除现有工作分配。</span><span class="sxs-lookup"><span data-stu-id="bb328-106">Delete an existing assignment.</span></span> <span data-ttu-id="bb328-107">只有课堂中的教师才能删除工作分配。</span><span class="sxs-lookup"><span data-stu-id="bb328-107">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb328-108">权限</span><span class="sxs-lookup"><span data-stu-id="bb328-108">Permissions</span></span>

<span data-ttu-id="bb328-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb328-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb328-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb328-111">Permission type</span></span>                        | <span data-ttu-id="bb328-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb328-112">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="bb328-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb328-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb328-114">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="bb328-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="bb328-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb328-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb328-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb328-116">Not Supported.</span></span>                                          |
| <span data-ttu-id="bb328-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb328-117">Application</span></span>                            | <span data-ttu-id="bb328-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb328-118">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="bb328-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb328-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bb328-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb328-120">Request headers</span></span>

| <span data-ttu-id="bb328-121">标头</span><span class="sxs-lookup"><span data-stu-id="bb328-121">Header</span></span>        | <span data-ttu-id="bb328-122">值</span><span class="sxs-lookup"><span data-stu-id="bb328-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="bb328-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb328-123">Authorization</span></span> | <span data-ttu-id="bb328-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb328-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb328-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb328-126">Request body</span></span>

<span data-ttu-id="bb328-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb328-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb328-128">响应</span><span class="sxs-lookup"><span data-stu-id="bb328-128">Response</span></span>

<span data-ttu-id="bb328-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bb328-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb328-131">示例</span><span class="sxs-lookup"><span data-stu-id="bb328-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb328-132">请求</span><span class="sxs-lookup"><span data-stu-id="bb328-132">Request</span></span>

<span data-ttu-id="bb328-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bb328-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bb328-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb328-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
# <a name="c"></a>[<span data-ttu-id="bb328-135">C#</span><span class="sxs-lookup"><span data-stu-id="bb328-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb328-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb328-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb328-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb328-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb328-138">Java</span><span class="sxs-lookup"><span data-stu-id="bb328-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="bb328-139">响应</span><span class="sxs-lookup"><span data-stu-id="bb328-139">Response</span></span>
<span data-ttu-id="bb328-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bb328-140">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


