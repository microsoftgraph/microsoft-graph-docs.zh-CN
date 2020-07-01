---
title: 删除 externalItem
description: 删除 externalItem。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: f9abe39baa29ba247994d4ea6ff8c30bd7f28f72
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006784"
---
# <a name="delete-externalitem"></a><span data-ttu-id="5d3b9-103">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="5d3b9-103">Delete externalItem</span></span>

<span data-ttu-id="5d3b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d3b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d3b9-105">删除[externalitem](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="5d3b9-105">Delete an [externalitem](../resources/externalitem.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="5d3b9-106">权限</span><span class="sxs-lookup"><span data-stu-id="5d3b9-106">Permissions</span></span>

<span data-ttu-id="5d3b9-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5d3b9-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d3b9-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d3b9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d3b9-109">Permission type</span></span>                        | <span data-ttu-id="5d3b9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d3b9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5d3b9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d3b9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d3b9-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d3b9-112">Not supported.</span></span> |
| <span data-ttu-id="5d3b9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d3b9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d3b9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d3b9-114">Not supported.</span></span> |
| <span data-ttu-id="5d3b9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d3b9-115">Application</span></span>                            | <span data-ttu-id="5d3b9-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d3b9-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d3b9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d3b9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="5d3b9-118">路径参数</span><span class="sxs-lookup"><span data-stu-id="5d3b9-118">Path parameters</span></span>

| <span data-ttu-id="5d3b9-119">参数</span><span class="sxs-lookup"><span data-stu-id="5d3b9-119">Parameter</span></span>     | <span data-ttu-id="5d3b9-120">类型</span><span class="sxs-lookup"><span data-stu-id="5d3b9-120">Type</span></span>   | <span data-ttu-id="5d3b9-121">说明</span><span class="sxs-lookup"><span data-stu-id="5d3b9-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="5d3b9-122">connection-id</span><span class="sxs-lookup"><span data-stu-id="5d3b9-122">connection-id</span></span> | <span data-ttu-id="5d3b9-123">string</span><span class="sxs-lookup"><span data-stu-id="5d3b9-123">string</span></span> | <span data-ttu-id="5d3b9-124">`id`包含[externalConnection](../resources/externalconnection.md)的属性</span><span class="sxs-lookup"><span data-stu-id="5d3b9-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="5d3b9-125">item-id</span><span class="sxs-lookup"><span data-stu-id="5d3b9-125">item-id</span></span>       | <span data-ttu-id="5d3b9-126">string</span><span class="sxs-lookup"><span data-stu-id="5d3b9-126">string</span></span> | <span data-ttu-id="5d3b9-127">ExternalItem 的开发人员提供的 `id` 属性[externalItem](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="5d3b9-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5d3b9-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d3b9-128">Request headers</span></span>

| <span data-ttu-id="5d3b9-129">名称</span><span class="sxs-lookup"><span data-stu-id="5d3b9-129">Name</span></span>          | <span data-ttu-id="5d3b9-130">说明</span><span class="sxs-lookup"><span data-stu-id="5d3b9-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5d3b9-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d3b9-131">Authorization</span></span> | <span data-ttu-id="5d3b9-132">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-132">Bearer {token}.</span></span> <span data-ttu-id="5d3b9-133">Required.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-133">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d3b9-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d3b9-134">Request body</span></span>

<span data-ttu-id="5d3b9-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5d3b9-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d3b9-136">响应</span><span class="sxs-lookup"><span data-stu-id="5d3b9-136">Response</span></span>

<span data-ttu-id="5d3b9-137">If successful, this method returns `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-137">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="5d3b9-138">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="5d3b9-138">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5d3b9-139">示例</span><span class="sxs-lookup"><span data-stu-id="5d3b9-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d3b9-140">请求</span><span class="sxs-lookup"><span data-stu-id="5d3b9-140">Request</span></span>

<span data-ttu-id="5d3b9-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5d3b9-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d3b9-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d3b9-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="5d3b9-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d3b9-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="5d3b9-144">C#</span><span class="sxs-lookup"><span data-stu-id="5d3b9-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d3b9-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d3b9-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="5d3b9-146">响应</span><span class="sxs-lookup"><span data-stu-id="5d3b9-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="5d3b9-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5d3b9-147">The following is an example of the response.</span></span>

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
