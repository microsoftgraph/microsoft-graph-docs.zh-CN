---
title: 从 onPremisesAgentGroup 中删除 publishedResource
description: 从[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象中删除[publishedResource](../resources/publishedresource.md)对象。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 4c93aeab74a8ef4191bd66354144e6746a5b5abf
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787581"
---
# <a name="remove-publishedresource-from-an-onpremisesagentgroup"></a><span data-ttu-id="231e4-103">从 onPremisesAgentGroup 中删除 publishedResource</span><span class="sxs-lookup"><span data-stu-id="231e4-103">Remove publishedResource from an onPremisesAgentGroup</span></span>

<span data-ttu-id="231e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="231e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="231e4-105">从[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象中删除[publishedResource](../resources/publishedresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="231e4-105">Remove a [publishedResource](../resources/publishedresource.md) object from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="231e4-106">权限</span><span class="sxs-lookup"><span data-stu-id="231e4-106">Permissions</span></span>

<span data-ttu-id="231e4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="231e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="231e4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="231e4-109">Permission type</span></span>                        | <span data-ttu-id="231e4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="231e4-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="231e4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="231e4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="231e4-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="231e4-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="231e4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="231e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="231e4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="231e4-114">Not supported.</span></span> |
| <span data-ttu-id="231e4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="231e4-115">Application</span></span>                            | <span data-ttu-id="231e4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="231e4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="231e4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="231e4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="231e4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="231e4-118">Request headers</span></span>

| <span data-ttu-id="231e4-119">名称</span><span class="sxs-lookup"><span data-stu-id="231e4-119">Name</span></span>          | <span data-ttu-id="231e4-120">说明</span><span class="sxs-lookup"><span data-stu-id="231e4-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="231e4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="231e4-121">Authorization</span></span> | <span data-ttu-id="231e4-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="231e4-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="231e4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="231e4-123">Request body</span></span>

<span data-ttu-id="231e4-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="231e4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="231e4-125">响应</span><span class="sxs-lookup"><span data-stu-id="231e4-125">Response</span></span>

<span data-ttu-id="231e4-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="231e4-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="231e4-127">示例</span><span class="sxs-lookup"><span data-stu-id="231e4-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="231e4-128">请求</span><span class="sxs-lookup"><span data-stu-id="231e4-128">Request</span></span>

<span data-ttu-id="231e4-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="231e4-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="231e4-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="231e4-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="231e4-131">C#</span><span class="sxs-lookup"><span data-stu-id="231e4-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onpremisesagentgroup-from-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="231e4-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="231e4-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="231e4-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="231e4-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="231e4-134">Java</span><span class="sxs-lookup"><span data-stu-id="231e4-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-onpremisesagentgroup-from-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="231e4-135">响应</span><span class="sxs-lookup"><span data-stu-id="231e4-135">Response</span></span>

<span data-ttu-id="231e4-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="231e4-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
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



