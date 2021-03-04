---
title: 删除案例
description: 删除 case 对象。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7c6958312795b304896904585ff0d5d66a74960a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446102"
---
# <a name="delete-case"></a><span data-ttu-id="f67c7-103">删除案例</span><span class="sxs-lookup"><span data-stu-id="f67c7-103">Delete case</span></span>

<span data-ttu-id="f67c7-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f67c7-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f67c7-105">删除 [case](../resources/ediscovery-case.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f67c7-105">Delete a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f67c7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f67c7-106">Permissions</span></span>

<span data-ttu-id="f67c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f67c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f67c7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f67c7-109">Permission type</span></span>|<span data-ttu-id="f67c7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f67c7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f67c7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f67c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f67c7-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f67c7-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f67c7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f67c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f67c7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f67c7-114">Not supported.</span></span>|
|<span data-ttu-id="f67c7-115">Application</span><span class="sxs-lookup"><span data-stu-id="f67c7-115">Application</span></span>|<span data-ttu-id="f67c7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f67c7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f67c7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f67c7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f67c7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f67c7-118">Request headers</span></span>

| <span data-ttu-id="f67c7-119">名称</span><span class="sxs-lookup"><span data-stu-id="f67c7-119">Name</span></span>          | <span data-ttu-id="f67c7-120">说明</span><span class="sxs-lookup"><span data-stu-id="f67c7-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f67c7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f67c7-121">Authorization</span></span> | <span data-ttu-id="f67c7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f67c7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f67c7-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f67c7-124">Request body</span></span>

<span data-ttu-id="f67c7-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f67c7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f67c7-126">响应</span><span class="sxs-lookup"><span data-stu-id="f67c7-126">Response</span></span>

<span data-ttu-id="f67c7-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f67c7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f67c7-128">示例</span><span class="sxs-lookup"><span data-stu-id="f67c7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f67c7-129">请求</span><span class="sxs-lookup"><span data-stu-id="f67c7-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f67c7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f67c7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_case"
}-->

```http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
```

# <a name="c"></a>[<span data-ttu-id="f67c7-131">C#</span><span class="sxs-lookup"><span data-stu-id="f67c7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f67c7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f67c7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f67c7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f67c7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-ediscoverycase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f67c7-134">Java</span><span class="sxs-lookup"><span data-stu-id="f67c7-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-ediscoverycase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f67c7-135">响应</span><span class="sxs-lookup"><span data-stu-id="f67c7-135">Response</span></span>

<span data-ttu-id="f67c7-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f67c7-136">The following is an example of the response.</span></span>

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
  "description": "Delete case",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
