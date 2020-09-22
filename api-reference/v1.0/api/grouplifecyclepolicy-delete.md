---
title: 删除 groupLifecyclePolicy
description: 删除 groupLifecyclePolicy。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b9f51c59806109a2c5ff673177807dce6f1d0276
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041888"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="70f0f-103">删除 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="70f0f-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="70f0f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70f0f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70f0f-105">删除 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="70f0f-105">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="70f0f-106">权限</span><span class="sxs-lookup"><span data-stu-id="70f0f-106">Permissions</span></span>

<span data-ttu-id="70f0f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70f0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70f0f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="70f0f-109">Permission type</span></span>      | <span data-ttu-id="70f0f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70f0f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70f0f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70f0f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="70f0f-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70f0f-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="70f0f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70f0f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70f0f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="70f0f-114">Not supported.</span></span>    |
|<span data-ttu-id="70f0f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="70f0f-115">Application</span></span> | <span data-ttu-id="70f0f-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70f0f-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70f0f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70f0f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="70f0f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="70f0f-118">Request headers</span></span>

| <span data-ttu-id="70f0f-119">名称</span><span class="sxs-lookup"><span data-stu-id="70f0f-119">Name</span></span> | <span data-ttu-id="70f0f-120">说明</span><span class="sxs-lookup"><span data-stu-id="70f0f-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="70f0f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="70f0f-121">Authorization</span></span> | <span data-ttu-id="70f0f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70f0f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70f0f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70f0f-124">Content-Type</span></span>  | <span data-ttu-id="70f0f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="70f0f-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="70f0f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="70f0f-126">Request body</span></span>
<span data-ttu-id="70f0f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="70f0f-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="70f0f-128">响应</span><span class="sxs-lookup"><span data-stu-id="70f0f-128">Response</span></span>

<span data-ttu-id="70f0f-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="70f0f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70f0f-131">示例</span><span class="sxs-lookup"><span data-stu-id="70f0f-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="70f0f-132">请求</span><span class="sxs-lookup"><span data-stu-id="70f0f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="70f0f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="70f0f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="70f0f-134">C#</span><span class="sxs-lookup"><span data-stu-id="70f0f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70f0f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70f0f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70f0f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70f0f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70f0f-137">Java</span><span class="sxs-lookup"><span data-stu-id="70f0f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="70f0f-138">响应</span><span class="sxs-lookup"><span data-stu-id="70f0f-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

