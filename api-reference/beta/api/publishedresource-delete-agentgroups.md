---
title: 从 onPremisesAgentGroup 中删除 publishedResource
description: 从[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象中删除[publishedResource](../resources/publishedresource.md)对象。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: f7ac461d17ac14f97c0043381ad565614c4c09d1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132459"
---
# <a name="remove-publishedresource-from-an-onpremisesagentgroup"></a><span data-ttu-id="bd415-103">从 onPremisesAgentGroup 中删除 publishedResource</span><span class="sxs-lookup"><span data-stu-id="bd415-103">Remove publishedResource from an onPremisesAgentGroup</span></span>

<span data-ttu-id="bd415-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd415-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd415-105">从[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象中删除[publishedResource](../resources/publishedresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bd415-105">Remove a [publishedResource](../resources/publishedresource.md) object from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd415-106">权限</span><span class="sxs-lookup"><span data-stu-id="bd415-106">Permissions</span></span>

<span data-ttu-id="bd415-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd415-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd415-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd415-109">Permission type</span></span>                        | <span data-ttu-id="bd415-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd415-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="bd415-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd415-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd415-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd415-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="bd415-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd415-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd415-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd415-114">Not supported.</span></span> |
| <span data-ttu-id="bd415-115">Application</span><span class="sxs-lookup"><span data-stu-id="bd415-115">Application</span></span>                            | <span data-ttu-id="bd415-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd415-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd415-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd415-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="bd415-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd415-118">Request headers</span></span>

| <span data-ttu-id="bd415-119">名称</span><span class="sxs-lookup"><span data-stu-id="bd415-119">Name</span></span>          | <span data-ttu-id="bd415-120">说明</span><span class="sxs-lookup"><span data-stu-id="bd415-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bd415-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd415-121">Authorization</span></span> | <span data-ttu-id="bd415-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="bd415-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd415-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd415-123">Request body</span></span>

<span data-ttu-id="bd415-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd415-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd415-125">响应</span><span class="sxs-lookup"><span data-stu-id="bd415-125">Response</span></span>

<span data-ttu-id="bd415-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bd415-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bd415-127">示例</span><span class="sxs-lookup"><span data-stu-id="bd415-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd415-128">请求</span><span class="sxs-lookup"><span data-stu-id="bd415-128">Request</span></span>

<span data-ttu-id="bd415-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bd415-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd415-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd415-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="bd415-131">C#</span><span class="sxs-lookup"><span data-stu-id="bd415-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onpremisesagentgroup-from-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd415-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd415-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd415-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd415-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd415-134">Java</span><span class="sxs-lookup"><span data-stu-id="bd415-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-onpremisesagentgroup-from-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd415-135">响应</span><span class="sxs-lookup"><span data-stu-id="bd415-135">Response</span></span>

<span data-ttu-id="bd415-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bd415-136">The following is an example of the response.</span></span>

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



