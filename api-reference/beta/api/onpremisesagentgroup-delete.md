---
title: 删除 onPremisesAgentGroup
description: 删除 **onPremisesAgentGroup** 对象。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e577d25d3dc2e9c6c17186f2ed585b320f1a8e82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017414"
---
# <a name="delete-onpremisesagentgroup"></a><span data-ttu-id="828ea-103">删除 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="828ea-103">Delete onPremisesAgentGroup</span></span>

<span data-ttu-id="828ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="828ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="828ea-105">删除 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="828ea-105">Delete an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="828ea-106">权限</span><span class="sxs-lookup"><span data-stu-id="828ea-106">Permissions</span></span>

<span data-ttu-id="828ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="828ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="828ea-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="828ea-109">Permission type</span></span>                        | <span data-ttu-id="828ea-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="828ea-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="828ea-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="828ea-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="828ea-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="828ea-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="828ea-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="828ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="828ea-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="828ea-114">Not supported.</span></span> |
| <span data-ttu-id="828ea-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="828ea-115">Application</span></span>                            | <span data-ttu-id="828ea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="828ea-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="828ea-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="828ea-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="828ea-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="828ea-118">Request headers</span></span>

| <span data-ttu-id="828ea-119">名称</span><span class="sxs-lookup"><span data-stu-id="828ea-119">Name</span></span>          | <span data-ttu-id="828ea-120">说明</span><span class="sxs-lookup"><span data-stu-id="828ea-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="828ea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="828ea-121">Authorization</span></span> | <span data-ttu-id="828ea-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="828ea-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="828ea-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="828ea-123">Request body</span></span>

<span data-ttu-id="828ea-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="828ea-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="828ea-125">响应</span><span class="sxs-lookup"><span data-stu-id="828ea-125">Response</span></span>

<span data-ttu-id="828ea-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="828ea-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="828ea-128">示例</span><span class="sxs-lookup"><span data-stu-id="828ea-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="828ea-129">请求</span><span class="sxs-lookup"><span data-stu-id="828ea-129">Request</span></span>

<span data-ttu-id="828ea-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="828ea-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="828ea-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="828ea-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesagentgroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/
```
# <a name="c"></a>[<span data-ttu-id="828ea-132">C#</span><span class="sxs-lookup"><span data-stu-id="828ea-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="828ea-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="828ea-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="828ea-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="828ea-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="828ea-135">响应</span><span class="sxs-lookup"><span data-stu-id="828ea-135">Response</span></span>

<span data-ttu-id="828ea-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="828ea-136">The following is an example of the response.</span></span>

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
  "description": "Delete onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


