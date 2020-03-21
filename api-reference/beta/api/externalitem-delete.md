---
title: 删除 externalItem
description: 删除 externalItem。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 263d04ed1b254a52d9eacab19997e40cdac4dc67
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892540"
---
# <a name="delete-externalitem"></a><span data-ttu-id="d61b4-103">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="d61b4-103">Delete externalItem</span></span>

<span data-ttu-id="d61b4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d61b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d61b4-105">删除[externalitem](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="d61b4-105">Delete an [externalitem](../resources/externalitem.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="d61b4-106">权限</span><span class="sxs-lookup"><span data-stu-id="d61b4-106">Permissions</span></span>

<span data-ttu-id="d61b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d61b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d61b4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d61b4-109">Permission type</span></span>                        | <span data-ttu-id="d61b4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d61b4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d61b4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d61b4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d61b4-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="d61b4-112">Not supported.</span></span> |
| <span data-ttu-id="d61b4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d61b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d61b4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d61b4-114">Not supported.</span></span> |
| <span data-ttu-id="d61b4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d61b4-115">Application</span></span>                            | <span data-ttu-id="d61b4-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d61b4-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d61b4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d61b4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="d61b4-118">路径参数</span><span class="sxs-lookup"><span data-stu-id="d61b4-118">Path parameters</span></span>

| <span data-ttu-id="d61b4-119">参数</span><span class="sxs-lookup"><span data-stu-id="d61b4-119">Parameter</span></span>     | <span data-ttu-id="d61b4-120">类型</span><span class="sxs-lookup"><span data-stu-id="d61b4-120">Type</span></span>   | <span data-ttu-id="d61b4-121">说明</span><span class="sxs-lookup"><span data-stu-id="d61b4-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="d61b4-122">connection-id</span><span class="sxs-lookup"><span data-stu-id="d61b4-122">connection-id</span></span> | <span data-ttu-id="d61b4-123">string</span><span class="sxs-lookup"><span data-stu-id="d61b4-123">string</span></span> | <span data-ttu-id="d61b4-124">包含`id` [externalConnection](../resources/externalconnection.md)的属性</span><span class="sxs-lookup"><span data-stu-id="d61b4-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="d61b4-125">item-id</span><span class="sxs-lookup"><span data-stu-id="d61b4-125">item-id</span></span>       | <span data-ttu-id="d61b4-126">string</span><span class="sxs-lookup"><span data-stu-id="d61b4-126">string</span></span> | <span data-ttu-id="d61b4-127">ExternalItem 的开发人员`id`提供的属性[externalItem](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="d61b4-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d61b4-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="d61b4-128">Request headers</span></span>

| <span data-ttu-id="d61b4-129">名称</span><span class="sxs-lookup"><span data-stu-id="d61b4-129">Name</span></span>          | <span data-ttu-id="d61b4-130">说明</span><span class="sxs-lookup"><span data-stu-id="d61b4-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d61b4-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="d61b4-131">Authorization</span></span> | <span data-ttu-id="d61b4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d61b4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d61b4-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="d61b4-134">Request body</span></span>

<span data-ttu-id="d61b4-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d61b4-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d61b4-136">响应</span><span class="sxs-lookup"><span data-stu-id="d61b4-136">Response</span></span>

<span data-ttu-id="d61b4-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d61b4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d61b4-139">示例</span><span class="sxs-lookup"><span data-stu-id="d61b4-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d61b4-140">请求</span><span class="sxs-lookup"><span data-stu-id="d61b4-140">Request</span></span>

<span data-ttu-id="d61b4-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d61b4-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d61b4-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d61b4-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="d61b4-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d61b4-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="d61b4-144">响应</span><span class="sxs-lookup"><span data-stu-id="d61b4-144">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="d61b4-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d61b4-145">The following is an example of the response.</span></span>

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
  "description": "Delete externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
