---
title: 删除 reviewSetQuery
description: 删除 reviewSetQuery 对象。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 01120e7702c2dc055ed0827d41b827a7330827bb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446024"
---
# <a name="delete-reviewsetquery"></a><span data-ttu-id="7e2f8-103">删除 reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="7e2f8-103">Delete reviewSetQuery</span></span>

<span data-ttu-id="7e2f8-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="7e2f8-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e2f8-105">删除 [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7e2f8-105">Delete a [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e2f8-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7e2f8-106">Permissions</span></span>

<span data-ttu-id="7e2f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e2f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e2f8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e2f8-109">Permission type</span></span>|<span data-ttu-id="7e2f8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e2f8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e2f8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e2f8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7e2f8-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e2f8-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="7e2f8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e2f8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e2f8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e2f8-114">Not supported.</span></span>|
|<span data-ttu-id="7e2f8-115">Application</span><span class="sxs-lookup"><span data-stu-id="7e2f8-115">Application</span></span>|<span data-ttu-id="7e2f8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e2f8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e2f8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e2f8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7e2f8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e2f8-118">Request headers</span></span>

| <span data-ttu-id="7e2f8-119">名称</span><span class="sxs-lookup"><span data-stu-id="7e2f8-119">Name</span></span>          | <span data-ttu-id="7e2f8-120">说明</span><span class="sxs-lookup"><span data-stu-id="7e2f8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7e2f8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e2f8-121">Authorization</span></span> | <span data-ttu-id="7e2f8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e2f8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e2f8-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e2f8-124">Request body</span></span>

<span data-ttu-id="7e2f8-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7e2f8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e2f8-126">响应</span><span class="sxs-lookup"><span data-stu-id="7e2f8-126">Response</span></span>

<span data-ttu-id="7e2f8-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7e2f8-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e2f8-129">示例</span><span class="sxs-lookup"><span data-stu-id="7e2f8-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7e2f8-130">请求</span><span class="sxs-lookup"><span data-stu-id="7e2f8-130">Request</span></span>

<span data-ttu-id="7e2f8-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e2f8-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e2f8-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e2f8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_reviewsetquery"
}-->

```http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
```
# <a name="c"></a>[<span data-ttu-id="7e2f8-133">C#</span><span class="sxs-lookup"><span data-stu-id="7e2f8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e2f8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e2f8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e2f8-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e2f8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e2f8-136">Java</span><span class="sxs-lookup"><span data-stu-id="7e2f8-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7e2f8-137">响应</span><span class="sxs-lookup"><span data-stu-id="7e2f8-137">Response</span></span>

<span data-ttu-id="7e2f8-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7e2f8-138">The following is an example of the response.</span></span>

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
  "description": "Delete reviewSetQuery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


