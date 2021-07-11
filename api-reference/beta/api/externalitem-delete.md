---
title: 删除 externalItem
description: 删除 externalItem。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 2506d03831637d27ebe3b874361f650e843f1cf4
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366799"
---
# <a name="delete-externalitem"></a><span data-ttu-id="531d7-103">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="531d7-103">Delete externalItem</span></span>

<span data-ttu-id="531d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="531d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="531d7-105">删除 [externalitem](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="531d7-105">Delete an [externalitem](../resources/externalitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="531d7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="531d7-106">Permissions</span></span>

<span data-ttu-id="531d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="531d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="531d7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="531d7-109">Permission type</span></span>                        | <span data-ttu-id="531d7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="531d7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="531d7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="531d7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="531d7-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="531d7-112">Not supported.</span></span> |
| <span data-ttu-id="531d7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="531d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="531d7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="531d7-114">Not supported.</span></span> |
| <span data-ttu-id="531d7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="531d7-115">Application</span></span>                            | <span data-ttu-id="531d7-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="531d7-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="531d7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="531d7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="531d7-118">路径参数</span><span class="sxs-lookup"><span data-stu-id="531d7-118">Path parameters</span></span>

| <span data-ttu-id="531d7-119">参数</span><span class="sxs-lookup"><span data-stu-id="531d7-119">Parameter</span></span>     | <span data-ttu-id="531d7-120">类型</span><span class="sxs-lookup"><span data-stu-id="531d7-120">Type</span></span>   | <span data-ttu-id="531d7-121">说明</span><span class="sxs-lookup"><span data-stu-id="531d7-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="531d7-122">connection-id</span><span class="sxs-lookup"><span data-stu-id="531d7-122">connection-id</span></span> | <span data-ttu-id="531d7-123">string</span><span class="sxs-lookup"><span data-stu-id="531d7-123">string</span></span> | <span data-ttu-id="531d7-124">`id`包含[externalConnection 的 属性](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="531d7-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="531d7-125">item-id</span><span class="sxs-lookup"><span data-stu-id="531d7-125">item-id</span></span>       | <span data-ttu-id="531d7-126">string</span><span class="sxs-lookup"><span data-stu-id="531d7-126">string</span></span> | <span data-ttu-id="531d7-127">由开发人员提供的 `id` [externalItem 属性](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="531d7-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="531d7-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="531d7-128">Request headers</span></span>

| <span data-ttu-id="531d7-129">名称</span><span class="sxs-lookup"><span data-stu-id="531d7-129">Name</span></span>          | <span data-ttu-id="531d7-130">说明</span><span class="sxs-lookup"><span data-stu-id="531d7-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="531d7-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="531d7-131">Authorization</span></span> | <span data-ttu-id="531d7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="531d7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="531d7-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="531d7-134">Request body</span></span>

<span data-ttu-id="531d7-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="531d7-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="531d7-136">响应</span><span class="sxs-lookup"><span data-stu-id="531d7-136">Response</span></span>

<span data-ttu-id="531d7-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="531d7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="531d7-139">示例</span><span class="sxs-lookup"><span data-stu-id="531d7-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="531d7-140">请求</span><span class="sxs-lookup"><span data-stu-id="531d7-140">Request</span></span>

<span data-ttu-id="531d7-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="531d7-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="531d7-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="531d7-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="531d7-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="531d7-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="531d7-144">C#</span><span class="sxs-lookup"><span data-stu-id="531d7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="531d7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="531d7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="531d7-146">Java</span><span class="sxs-lookup"><span data-stu-id="531d7-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="531d7-147">响应</span><span class="sxs-lookup"><span data-stu-id="531d7-147">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="531d7-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="531d7-148">The following is an example of the response.</span></span>

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


