---
title: 删除 educationCategory
description: 删除现有类别。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4bf5777ee48f4701a3a0ae29f1da9b9f9ab26269
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951700"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="246ef-103">删除 educationCategory</span><span class="sxs-lookup"><span data-stu-id="246ef-103">Delete educationCategory</span></span>

<span data-ttu-id="246ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="246ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="246ef-105">删除现有类别。</span><span class="sxs-lookup"><span data-stu-id="246ef-105">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="246ef-106">权限</span><span class="sxs-lookup"><span data-stu-id="246ef-106">Permissions</span></span>

<span data-ttu-id="246ef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="246ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="246ef-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="246ef-109">Permission type</span></span>                        | <span data-ttu-id="246ef-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="246ef-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="246ef-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="246ef-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="246ef-112">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="246ef-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="246ef-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="246ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="246ef-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="246ef-114">Not Supported.</span></span>                                          |
| <span data-ttu-id="246ef-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="246ef-115">Application</span></span>                            | <span data-ttu-id="246ef-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="246ef-116">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="246ef-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="246ef-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="246ef-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="246ef-118">Request headers</span></span>

| <span data-ttu-id="246ef-119">标头</span><span class="sxs-lookup"><span data-stu-id="246ef-119">Header</span></span>        | <span data-ttu-id="246ef-120">值</span><span class="sxs-lookup"><span data-stu-id="246ef-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="246ef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="246ef-121">Authorization</span></span> | <span data-ttu-id="246ef-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="246ef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="246ef-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="246ef-124">Request body</span></span>

<span data-ttu-id="246ef-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="246ef-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="246ef-126">响应</span><span class="sxs-lookup"><span data-stu-id="246ef-126">Response</span></span>

<span data-ttu-id="246ef-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="246ef-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="246ef-129">示例</span><span class="sxs-lookup"><span data-stu-id="246ef-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="246ef-130">请求</span><span class="sxs-lookup"><span data-stu-id="246ef-130">Request</span></span>

<span data-ttu-id="246ef-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="246ef-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="246ef-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="246ef-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment_2"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
# <a name="c"></a>[<span data-ttu-id="246ef-133">C#</span><span class="sxs-lookup"><span data-stu-id="246ef-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="246ef-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="246ef-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="246ef-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="246ef-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="246ef-136">Java</span><span class="sxs-lookup"><span data-stu-id="246ef-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="246ef-137">响应</span><span class="sxs-lookup"><span data-stu-id="246ef-137">Response</span></span>

<span data-ttu-id="246ef-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="246ef-138">The following is an example of the response.</span></span> 

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


