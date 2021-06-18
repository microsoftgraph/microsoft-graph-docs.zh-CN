---
title: 删除 educationCategory
description: 删除现有类别。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ba6a68358f91e2f965bb5fe8a39145ee20295d93
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992864"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="642ca-103">删除 educationCategory</span><span class="sxs-lookup"><span data-stu-id="642ca-103">Delete educationCategory</span></span>

<span data-ttu-id="642ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="642ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="642ca-105">删除现有 [类别](../resources/educationcategory.md)。</span><span class="sxs-lookup"><span data-stu-id="642ca-105">Delete an existing [category](../resources/educationcategory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="642ca-106">权限</span><span class="sxs-lookup"><span data-stu-id="642ca-106">Permissions</span></span>

<span data-ttu-id="642ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="642ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="642ca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="642ca-109">Permission type</span></span>                        | <span data-ttu-id="642ca-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="642ca-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="642ca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="642ca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="642ca-112">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="642ca-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="642ca-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="642ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="642ca-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="642ca-114">Not Supported.</span></span>                                          |
| <span data-ttu-id="642ca-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="642ca-115">Application</span></span>                            | <span data-ttu-id="642ca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="642ca-116">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="642ca-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="642ca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="642ca-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="642ca-118">Request headers</span></span>

| <span data-ttu-id="642ca-119">标头</span><span class="sxs-lookup"><span data-stu-id="642ca-119">Header</span></span>        | <span data-ttu-id="642ca-120">值</span><span class="sxs-lookup"><span data-stu-id="642ca-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="642ca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="642ca-121">Authorization</span></span> | <span data-ttu-id="642ca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="642ca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="642ca-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="642ca-124">Request body</span></span>

<span data-ttu-id="642ca-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="642ca-125">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="642ca-126">响应</span><span class="sxs-lookup"><span data-stu-id="642ca-126">Response</span></span>

<span data-ttu-id="642ca-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="642ca-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="642ca-129">示例</span><span class="sxs-lookup"><span data-stu-id="642ca-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="642ca-130">请求</span><span class="sxs-lookup"><span data-stu-id="642ca-130">Request</span></span>

<span data-ttu-id="642ca-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="642ca-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="642ca-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="642ca-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment_2"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/classes/c42f493f-42b4-4e7d-8148-af894cbc518b/assignmentCategories/b93d3b6b-360c-45c0-8764-e8bb622a9504
```
# <a name="c"></a>[<span data-ttu-id="642ca-133">C#</span><span class="sxs-lookup"><span data-stu-id="642ca-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="642ca-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="642ca-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="642ca-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="642ca-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="642ca-136">Java</span><span class="sxs-lookup"><span data-stu-id="642ca-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="642ca-137">响应</span><span class="sxs-lookup"><span data-stu-id="642ca-137">Response</span></span>

<span data-ttu-id="642ca-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="642ca-138">The following is an example of the response.</span></span> 

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


