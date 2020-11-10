---
title: 删除 educationRubric
description: 删除 educationRubric 对象。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a697de8117263392bbd055096a07d03c89579ec8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966040"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="3667e-103">删除 educationRubric</span><span class="sxs-lookup"><span data-stu-id="3667e-103">Delete educationRubric</span></span>

<span data-ttu-id="3667e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3667e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3667e-105">删除 [educationRubric](../resources/educationrubric.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3667e-105">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3667e-106">权限</span><span class="sxs-lookup"><span data-stu-id="3667e-106">Permissions</span></span>

<span data-ttu-id="3667e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3667e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3667e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3667e-109">Permission type</span></span>                        | <span data-ttu-id="3667e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3667e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3667e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3667e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3667e-112">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="3667e-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="3667e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3667e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3667e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3667e-114">Not supported.</span></span> |
| <span data-ttu-id="3667e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3667e-115">Application</span></span>                            | <span data-ttu-id="3667e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3667e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3667e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3667e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3667e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3667e-118">Request headers</span></span>

| <span data-ttu-id="3667e-119">名称</span><span class="sxs-lookup"><span data-stu-id="3667e-119">Name</span></span>          | <span data-ttu-id="3667e-120">说明</span><span class="sxs-lookup"><span data-stu-id="3667e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3667e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3667e-121">Authorization</span></span> | <span data-ttu-id="3667e-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="3667e-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3667e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3667e-123">Request body</span></span>

<span data-ttu-id="3667e-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3667e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3667e-125">响应</span><span class="sxs-lookup"><span data-stu-id="3667e-125">Response</span></span>

<span data-ttu-id="3667e-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3667e-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3667e-128">示例</span><span class="sxs-lookup"><span data-stu-id="3667e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3667e-129">请求</span><span class="sxs-lookup"><span data-stu-id="3667e-129">Request</span></span>

<span data-ttu-id="3667e-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3667e-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3667e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3667e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/rubrics/{id}
```
# <a name="c"></a>[<span data-ttu-id="3667e-132">C#</span><span class="sxs-lookup"><span data-stu-id="3667e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3667e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3667e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3667e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3667e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3667e-135">Java</span><span class="sxs-lookup"><span data-stu-id="3667e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationrubric-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3667e-136">响应</span><span class="sxs-lookup"><span data-stu-id="3667e-136">Response</span></span>

<span data-ttu-id="3667e-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3667e-137">The following is an example of the response.</span></span>

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


