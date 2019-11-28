---
title: 删除 externalItem
description: 删除 externalItem 或 externalFile。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 34a34c3913ccf4da490a79b2449e06ff45fc8512
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636811"
---
# <a name="delete-externalitem"></a><span data-ttu-id="599e0-103">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="599e0-103">Delete externalItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="599e0-104">删除[externalitem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)。</span><span class="sxs-lookup"><span data-stu-id="599e0-104">Delete an [externalitem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="599e0-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="599e0-105">Permissions</span></span>

<span data-ttu-id="599e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="599e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="599e0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="599e0-108">Permission type</span></span>                        | <span data-ttu-id="599e0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="599e0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="599e0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="599e0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="599e0-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="599e0-111">Not supported.</span></span> |
| <span data-ttu-id="599e0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="599e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="599e0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="599e0-113">Not supported.</span></span> |
| <span data-ttu-id="599e0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="599e0-114">Application</span></span>                            | <span data-ttu-id="599e0-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="599e0-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="599e0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="599e0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="599e0-117">路径参数</span><span class="sxs-lookup"><span data-stu-id="599e0-117">Path parameters</span></span>

| <span data-ttu-id="599e0-118">参数</span><span class="sxs-lookup"><span data-stu-id="599e0-118">Parameter</span></span>     | <span data-ttu-id="599e0-119">类型</span><span class="sxs-lookup"><span data-stu-id="599e0-119">Type</span></span>   | <span data-ttu-id="599e0-120">说明</span><span class="sxs-lookup"><span data-stu-id="599e0-120">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="599e0-121">connection-id</span><span class="sxs-lookup"><span data-stu-id="599e0-121">connection-id</span></span> | <span data-ttu-id="599e0-122">string</span><span class="sxs-lookup"><span data-stu-id="599e0-122">string</span></span> | <span data-ttu-id="599e0-123">包含`id` [externalConnection](../resources/externalconnection.md)的属性</span><span class="sxs-lookup"><span data-stu-id="599e0-123">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="599e0-124">item-id</span><span class="sxs-lookup"><span data-stu-id="599e0-124">item-id</span></span>       | <span data-ttu-id="599e0-125">string</span><span class="sxs-lookup"><span data-stu-id="599e0-125">string</span></span> | <span data-ttu-id="599e0-126">开发人员提供`id`的[externalItem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)属性。</span><span class="sxs-lookup"><span data-stu-id="599e0-126">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="599e0-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="599e0-127">Request headers</span></span>

| <span data-ttu-id="599e0-128">名称</span><span class="sxs-lookup"><span data-stu-id="599e0-128">Name</span></span>          | <span data-ttu-id="599e0-129">说明</span><span class="sxs-lookup"><span data-stu-id="599e0-129">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="599e0-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="599e0-130">Authorization</span></span> | <span data-ttu-id="599e0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="599e0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="599e0-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="599e0-133">Request body</span></span>

<span data-ttu-id="599e0-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="599e0-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="599e0-135">响应</span><span class="sxs-lookup"><span data-stu-id="599e0-135">Response</span></span>

<span data-ttu-id="599e0-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="599e0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="599e0-138">示例</span><span class="sxs-lookup"><span data-stu-id="599e0-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="599e0-139">请求</span><span class="sxs-lookup"><span data-stu-id="599e0-139">Request</span></span>

<span data-ttu-id="599e0-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="599e0-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="599e0-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="599e0-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-ctabobjc"></a>[<span data-ttu-id="599e0-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="599e0-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="599e0-143">响应</span><span class="sxs-lookup"><span data-stu-id="599e0-143">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="599e0-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="599e0-144">The following is an example of the response.</span></span>

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
