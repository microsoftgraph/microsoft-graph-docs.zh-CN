---
title: 删除 publishedResource
description: 删除 [publishedResource](../resources/publishedresource.md) 对象。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9792f8a66d4e4d5e65da8dcca74d0fb2dbff577f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973410"
---
# <a name="delete-publishedresource"></a><span data-ttu-id="45a6d-103">删除 publishedResource</span><span class="sxs-lookup"><span data-stu-id="45a6d-103">Delete publishedResource</span></span>

<span data-ttu-id="45a6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45a6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45a6d-105">删除 [publishedResource](../resources/publishedresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45a6d-105">Delete a [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="45a6d-106">权限</span><span class="sxs-lookup"><span data-stu-id="45a6d-106">Permissions</span></span>

<span data-ttu-id="45a6d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45a6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="45a6d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="45a6d-109">Permission type</span></span>                        | <span data-ttu-id="45a6d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45a6d-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="45a6d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45a6d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="45a6d-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45a6d-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="45a6d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45a6d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45a6d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="45a6d-114">Not supported.</span></span> |
| <span data-ttu-id="45a6d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="45a6d-115">Application</span></span>                            | <span data-ttu-id="45a6d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="45a6d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45a6d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45a6d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="45a6d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="45a6d-118">Request headers</span></span>

| <span data-ttu-id="45a6d-119">名称</span><span class="sxs-lookup"><span data-stu-id="45a6d-119">Name</span></span>          | <span data-ttu-id="45a6d-120">说明</span><span class="sxs-lookup"><span data-stu-id="45a6d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="45a6d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="45a6d-121">Authorization</span></span> | <span data-ttu-id="45a6d-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="45a6d-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="45a6d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="45a6d-123">Request body</span></span>

<span data-ttu-id="45a6d-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="45a6d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45a6d-125">响应</span><span class="sxs-lookup"><span data-stu-id="45a6d-125">Response</span></span>

<span data-ttu-id="45a6d-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="45a6d-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45a6d-128">示例</span><span class="sxs-lookup"><span data-stu-id="45a6d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45a6d-129">请求</span><span class="sxs-lookup"><span data-stu-id="45a6d-129">Request</span></span>

<span data-ttu-id="45a6d-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="45a6d-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45a6d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="45a6d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="45a6d-132">C#</span><span class="sxs-lookup"><span data-stu-id="45a6d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45a6d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45a6d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45a6d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45a6d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45a6d-135">Java</span><span class="sxs-lookup"><span data-stu-id="45a6d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="45a6d-136">响应</span><span class="sxs-lookup"><span data-stu-id="45a6d-136">Response</span></span>

<span data-ttu-id="45a6d-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="45a6d-137">The following is an example of the response.</span></span>

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
  "description": "Delete publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


