---
title: 从 educationAssignment 中删除 educationRubric
description: 从 educationAssignment 中删除 educationRubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 119fe854c1bc04f850e89fcaf9dd8460b87ac95d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966601"
---
# <a name="remove-educationrubric-from-educationassignment"></a><span data-ttu-id="076ad-103">从 educationAssignment 中删除 educationRubric</span><span class="sxs-lookup"><span data-stu-id="076ad-103">Remove educationRubric from educationAssignment</span></span>

<span data-ttu-id="076ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="076ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="076ad-105">从[educationAssignment](../resources/educationassignment.md)中删除[educationRubric](../resources/educationrubric.md) 。</span><span class="sxs-lookup"><span data-stu-id="076ad-105">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>  <span data-ttu-id="076ad-106">这不会删除 rubric 本身。</span><span class="sxs-lookup"><span data-stu-id="076ad-106">This does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="076ad-107">权限</span><span class="sxs-lookup"><span data-stu-id="076ad-107">Permissions</span></span>

<span data-ttu-id="076ad-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="076ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="076ad-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="076ad-110">Permission type</span></span>                        | <span data-ttu-id="076ad-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="076ad-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="076ad-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="076ad-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="076ad-113">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="076ad-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="076ad-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="076ad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="076ad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="076ad-115">Not supported.</span></span> |
| <span data-ttu-id="076ad-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="076ad-116">Application</span></span>                            | <span data-ttu-id="076ad-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="076ad-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="076ad-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="076ad-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="076ad-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="076ad-119">Request headers</span></span>

| <span data-ttu-id="076ad-120">名称</span><span class="sxs-lookup"><span data-stu-id="076ad-120">Name</span></span>          | <span data-ttu-id="076ad-121">说明</span><span class="sxs-lookup"><span data-stu-id="076ad-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="076ad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="076ad-122">Authorization</span></span> | <span data-ttu-id="076ad-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="076ad-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="076ad-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="076ad-124">Request body</span></span>

<span data-ttu-id="076ad-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="076ad-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="076ad-126">响应</span><span class="sxs-lookup"><span data-stu-id="076ad-126">Response</span></span>

<span data-ttu-id="076ad-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="076ad-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="076ad-129">示例</span><span class="sxs-lookup"><span data-stu-id="076ad-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="076ad-130">请求</span><span class="sxs-lookup"><span data-stu-id="076ad-130">Request</span></span>

<span data-ttu-id="076ad-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="076ad-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="076ad-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="076ad-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric/$ref
```
# <a name="c"></a>[<span data-ttu-id="076ad-133">C#</span><span class="sxs-lookup"><span data-stu-id="076ad-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="076ad-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="076ad-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="076ad-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="076ad-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="076ad-136">Java</span><span class="sxs-lookup"><span data-stu-id="076ad-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationrubric-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="076ad-137">响应</span><span class="sxs-lookup"><span data-stu-id="076ad-137">Response</span></span>

<span data-ttu-id="076ad-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="076ad-138">The following is an example of the response.</span></span>

> <span data-ttu-id="076ad-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="076ad-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


