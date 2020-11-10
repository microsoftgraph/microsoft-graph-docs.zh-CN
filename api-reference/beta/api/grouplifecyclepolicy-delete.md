---
title: 删除 groupLifecyclePolicy
description: 删除 groupLifecyclePolicy。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2fd9ee7711a8401796694c7ad4d8ed80590cab1e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953696"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="fc938-103">删除 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="fc938-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="fc938-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc938-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc938-105">删除 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="fc938-105">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fc938-106">权限</span><span class="sxs-lookup"><span data-stu-id="fc938-106">Permissions</span></span>

<span data-ttu-id="fc938-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc938-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc938-109">Permission type</span></span>      | <span data-ttu-id="fc938-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc938-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc938-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc938-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc938-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc938-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="fc938-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc938-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc938-114">不支持</span><span class="sxs-lookup"><span data-stu-id="fc938-114">Not supported</span></span> |
|<span data-ttu-id="fc938-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc938-115">Application</span></span> | <span data-ttu-id="fc938-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc938-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc938-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc938-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="fc938-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc938-118">Request headers</span></span>

| <span data-ttu-id="fc938-119">名称</span><span class="sxs-lookup"><span data-stu-id="fc938-119">Name</span></span> | <span data-ttu-id="fc938-120">说明</span><span class="sxs-lookup"><span data-stu-id="fc938-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="fc938-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc938-121">Authorization</span></span> | <span data-ttu-id="fc938-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fc938-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc938-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc938-124">Content-Type</span></span>  | <span data-ttu-id="fc938-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc938-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc938-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc938-126">Request body</span></span>
<span data-ttu-id="fc938-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fc938-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="fc938-128">响应</span><span class="sxs-lookup"><span data-stu-id="fc938-128">Response</span></span>

<span data-ttu-id="fc938-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fc938-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc938-131">示例</span><span class="sxs-lookup"><span data-stu-id="fc938-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fc938-132">请求</span><span class="sxs-lookup"><span data-stu-id="fc938-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fc938-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc938-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="fc938-134">C#</span><span class="sxs-lookup"><span data-stu-id="fc938-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc938-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc938-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc938-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc938-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc938-137">Java</span><span class="sxs-lookup"><span data-stu-id="fc938-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fc938-138">响应</span><span class="sxs-lookup"><span data-stu-id="fc938-138">Response</span></span>

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
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


