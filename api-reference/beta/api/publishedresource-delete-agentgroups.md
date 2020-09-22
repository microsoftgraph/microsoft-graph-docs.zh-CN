---
title: 从 onPremisesAgentGroup 中删除 publishedResource
description: 从[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象中删除一个[publishedResource](../resources/publishedresource.md)对象。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7dbf0d364b4671197fe5baa704cf7a60862fceb8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047159"
---
# <a name="remove-publishedresource-from-an-onpremisesagentgroup"></a><span data-ttu-id="8abef-103">从 onPremisesAgentGroup 中删除 publishedResource</span><span class="sxs-lookup"><span data-stu-id="8abef-103">Remove publishedResource from an onPremisesAgentGroup</span></span>

<span data-ttu-id="8abef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8abef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8abef-105">从[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象中删除一个[publishedResource](../resources/publishedresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8abef-105">Remove a [publishedResource](../resources/publishedresource.md) object from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8abef-106">权限</span><span class="sxs-lookup"><span data-stu-id="8abef-106">Permissions</span></span>

<span data-ttu-id="8abef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8abef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8abef-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8abef-109">Permission type</span></span>                        | <span data-ttu-id="8abef-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8abef-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="8abef-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8abef-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8abef-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8abef-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="8abef-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8abef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8abef-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8abef-114">Not supported.</span></span> |
| <span data-ttu-id="8abef-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8abef-115">Application</span></span>                            | <span data-ttu-id="8abef-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8abef-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8abef-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8abef-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8abef-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8abef-118">Request headers</span></span>

| <span data-ttu-id="8abef-119">名称</span><span class="sxs-lookup"><span data-stu-id="8abef-119">Name</span></span>          | <span data-ttu-id="8abef-120">说明</span><span class="sxs-lookup"><span data-stu-id="8abef-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8abef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8abef-121">Authorization</span></span> | <span data-ttu-id="8abef-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="8abef-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8abef-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8abef-123">Request body</span></span>

<span data-ttu-id="8abef-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8abef-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8abef-125">响应</span><span class="sxs-lookup"><span data-stu-id="8abef-125">Response</span></span>

<span data-ttu-id="8abef-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8abef-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8abef-127">示例</span><span class="sxs-lookup"><span data-stu-id="8abef-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8abef-128">请求</span><span class="sxs-lookup"><span data-stu-id="8abef-128">Request</span></span>

<span data-ttu-id="8abef-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8abef-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8abef-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8abef-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="8abef-131">C#</span><span class="sxs-lookup"><span data-stu-id="8abef-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onpremisesagentgroup-from-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8abef-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8abef-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8abef-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8abef-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8abef-134">响应</span><span class="sxs-lookup"><span data-stu-id="8abef-134">Response</span></span>

<span data-ttu-id="8abef-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8abef-135">The following is an example of the response.</span></span>

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


