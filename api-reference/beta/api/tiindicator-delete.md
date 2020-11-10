---
title: 删除威胁情报指标
description: 删除 tiIndicator 对象。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 579b46e54c51879e6e037b06bab40eee99d3b865
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977772"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="58591-103">删除威胁情报指标</span><span class="sxs-lookup"><span data-stu-id="58591-103">Delete threat intelligence indicator</span></span>

<span data-ttu-id="58591-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58591-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58591-105">删除 [tiIndicator](../resources/tiindicator.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58591-105">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="58591-106">权限</span><span class="sxs-lookup"><span data-stu-id="58591-106">Permissions</span></span>

<span data-ttu-id="58591-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58591-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58591-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="58591-109">Permission type</span></span>                        | <span data-ttu-id="58591-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="58591-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="58591-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58591-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="58591-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="58591-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="58591-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58591-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58591-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="58591-114">Not supported.</span></span> |
| <span data-ttu-id="58591-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="58591-115">Application</span></span>                            | <span data-ttu-id="58591-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="58591-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="58591-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58591-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="58591-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="58591-118">Request headers</span></span>

| <span data-ttu-id="58591-119">名称</span><span class="sxs-lookup"><span data-stu-id="58591-119">Name</span></span>          | <span data-ttu-id="58591-120">说明</span><span class="sxs-lookup"><span data-stu-id="58591-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="58591-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="58591-121">Authorization</span></span> | <span data-ttu-id="58591-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="58591-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="58591-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="58591-123">Request body</span></span>

<span data-ttu-id="58591-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="58591-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58591-125">响应</span><span class="sxs-lookup"><span data-stu-id="58591-125">Response</span></span>

<span data-ttu-id="58591-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="58591-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58591-128">示例</span><span class="sxs-lookup"><span data-stu-id="58591-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="58591-129">请求</span><span class="sxs-lookup"><span data-stu-id="58591-129">Request</span></span>

<span data-ttu-id="58591-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="58591-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="58591-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="58591-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="c"></a>[<span data-ttu-id="58591-132">C#</span><span class="sxs-lookup"><span data-stu-id="58591-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58591-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58591-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58591-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58591-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58591-135">Java</span><span class="sxs-lookup"><span data-stu-id="58591-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="58591-136">响应</span><span class="sxs-lookup"><span data-stu-id="58591-136">Response</span></span>

<span data-ttu-id="58591-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="58591-137">The following is an example of the response.</span></span>

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
  "description": "Delete tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


