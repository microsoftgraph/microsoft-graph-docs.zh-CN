---
title: 删除 groupLifecyclePolicy
description: 删除 groupLifecyclePolicy。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6ad18eb72988318a8639c1d48120d2ba3320064f
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123724"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="b5e98-103">删除 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b5e98-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="b5e98-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5e98-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5e98-105">删除 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="b5e98-105">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b5e98-106">权限</span><span class="sxs-lookup"><span data-stu-id="b5e98-106">Permissions</span></span>

<span data-ttu-id="b5e98-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5e98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5e98-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5e98-109">Permission type</span></span>      | <span data-ttu-id="b5e98-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5e98-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5e98-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5e98-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b5e98-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5e98-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5e98-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5e98-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5e98-114">不支持</span><span class="sxs-lookup"><span data-stu-id="b5e98-114">Not supported</span></span> |
|<span data-ttu-id="b5e98-115">Application</span><span class="sxs-lookup"><span data-stu-id="b5e98-115">Application</span></span> | <span data-ttu-id="b5e98-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5e98-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5e98-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5e98-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="b5e98-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5e98-118">Request headers</span></span>

| <span data-ttu-id="b5e98-119">名称</span><span class="sxs-lookup"><span data-stu-id="b5e98-119">Name</span></span> | <span data-ttu-id="b5e98-120">说明</span><span class="sxs-lookup"><span data-stu-id="b5e98-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b5e98-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5e98-121">Authorization</span></span> | <span data-ttu-id="b5e98-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5e98-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b5e98-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5e98-124">Content-Type</span></span>  | <span data-ttu-id="b5e98-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5e98-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5e98-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5e98-126">Request body</span></span>
<span data-ttu-id="b5e98-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5e98-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b5e98-128">响应</span><span class="sxs-lookup"><span data-stu-id="b5e98-128">Response</span></span>

<span data-ttu-id="b5e98-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b5e98-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5e98-131">示例</span><span class="sxs-lookup"><span data-stu-id="b5e98-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b5e98-132">请求</span><span class="sxs-lookup"><span data-stu-id="b5e98-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b5e98-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5e98-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="b5e98-134">C#</span><span class="sxs-lookup"><span data-stu-id="b5e98-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5e98-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5e98-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5e98-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5e98-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b5e98-137">响应</span><span class="sxs-lookup"><span data-stu-id="b5e98-137">Response</span></span>

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
