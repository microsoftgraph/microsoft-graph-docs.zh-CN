---
title: 从 onPremisesAgentGroup 中删除 publishedResource
description: 从[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象中删除一个[publishedResource](../resources/publishedresource.md)对象。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e300f57d58dcb0d9b32f17fa603b50df9aeb4c1
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200185"
---
# <a name="remove-publishedresource-from-an-onpremisesagentgroup"></a><span data-ttu-id="f2842-103">从 onPremisesAgentGroup 中删除 publishedResource</span><span class="sxs-lookup"><span data-stu-id="f2842-103">Remove publishedResource from an onPremisesAgentGroup</span></span>

<span data-ttu-id="f2842-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2842-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2842-105">从[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象中删除一个[publishedResource](../resources/publishedresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f2842-105">Remove a [publishedResource](../resources/publishedresource.md) object from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2842-106">权限</span><span class="sxs-lookup"><span data-stu-id="f2842-106">Permissions</span></span>

<span data-ttu-id="f2842-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2842-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2842-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2842-109">Permission type</span></span>                        | <span data-ttu-id="f2842-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2842-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="f2842-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2842-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2842-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2842-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="f2842-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2842-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2842-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2842-114">Not supported.</span></span> |
| <span data-ttu-id="f2842-115">Application</span><span class="sxs-lookup"><span data-stu-id="f2842-115">Application</span></span>                            | <span data-ttu-id="f2842-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2842-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2842-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2842-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f2842-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2842-118">Request headers</span></span>

| <span data-ttu-id="f2842-119">名称</span><span class="sxs-lookup"><span data-stu-id="f2842-119">Name</span></span>          | <span data-ttu-id="f2842-120">说明</span><span class="sxs-lookup"><span data-stu-id="f2842-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f2842-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2842-121">Authorization</span></span> | <span data-ttu-id="f2842-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="f2842-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2842-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2842-123">Request body</span></span>

<span data-ttu-id="f2842-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f2842-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2842-125">响应</span><span class="sxs-lookup"><span data-stu-id="f2842-125">Response</span></span>

<span data-ttu-id="f2842-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f2842-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f2842-127">示例</span><span class="sxs-lookup"><span data-stu-id="f2842-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2842-128">请求</span><span class="sxs-lookup"><span data-stu-id="f2842-128">Request</span></span>

<span data-ttu-id="f2842-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f2842-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f2842-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2842-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="f2842-131">C#</span><span class="sxs-lookup"><span data-stu-id="f2842-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onpremisesagentgroup-from-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2842-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2842-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2842-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2842-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f2842-134">响应</span><span class="sxs-lookup"><span data-stu-id="f2842-134">Response</span></span>

<span data-ttu-id="f2842-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f2842-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
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
