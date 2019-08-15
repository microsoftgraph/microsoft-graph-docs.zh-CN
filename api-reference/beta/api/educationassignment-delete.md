---
title: 删除 educationAssignment
description: 删除现有工作分配。 只有课堂中的教师才能删除工作分配。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c1846f61884b35c6a8f460615aaacd441aabfd38
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416553"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="2e63d-104">删除 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="2e63d-104">Delete educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e63d-105">删除现有工作分配。</span><span class="sxs-lookup"><span data-stu-id="2e63d-105">Delete an existing assignment.</span></span> <span data-ttu-id="2e63d-106">只有课堂中的教师才能删除工作分配。</span><span class="sxs-lookup"><span data-stu-id="2e63d-106">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e63d-107">权限</span><span class="sxs-lookup"><span data-stu-id="2e63d-107">Permissions</span></span>

<span data-ttu-id="2e63d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e63d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e63d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e63d-110">Permission type</span></span>                        | <span data-ttu-id="2e63d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e63d-111">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="2e63d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e63d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e63d-113">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="2e63d-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="2e63d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e63d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e63d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e63d-115">Not Supported.</span></span>                                          |
| <span data-ttu-id="2e63d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e63d-116">Application</span></span>                            | <span data-ttu-id="2e63d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e63d-117">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="2e63d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e63d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2e63d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e63d-119">Request headers</span></span>

| <span data-ttu-id="2e63d-120">标头</span><span class="sxs-lookup"><span data-stu-id="2e63d-120">Header</span></span>        | <span data-ttu-id="2e63d-121">值</span><span class="sxs-lookup"><span data-stu-id="2e63d-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="2e63d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e63d-122">Authorization</span></span> | <span data-ttu-id="2e63d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2e63d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e63d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e63d-125">Request body</span></span>

<span data-ttu-id="2e63d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2e63d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e63d-127">响应</span><span class="sxs-lookup"><span data-stu-id="2e63d-127">Response</span></span>

<span data-ttu-id="2e63d-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2e63d-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e63d-130">示例</span><span class="sxs-lookup"><span data-stu-id="2e63d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e63d-131">请求</span><span class="sxs-lookup"><span data-stu-id="2e63d-131">Request</span></span>

<span data-ttu-id="2e63d-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2e63d-132">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2e63d-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2e63d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2e63d-134">C#</span><span class="sxs-lookup"><span data-stu-id="2e63d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e63d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e63d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2e63d-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="2e63d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2e63d-137">响应</span><span class="sxs-lookup"><span data-stu-id="2e63d-137">Response</span></span>
<span data-ttu-id="2e63d-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2e63d-138">The following is an example of the response.</span></span> 


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
