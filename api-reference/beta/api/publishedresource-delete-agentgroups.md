---
title: 从 onPremisesAgentGroup 中删除 publishedResource
description: 从[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象中删除一个[publishedResource](../resources/publishedresource.md)对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 667ab45f08ed16abf471f626e0d9f09716f3c34d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342192"
---
# <a name="remove-publishedresource-from-an-onpremisesagentgroup"></a><span data-ttu-id="24c12-103">从 onPremisesAgentGroup 中删除 publishedResource</span><span class="sxs-lookup"><span data-stu-id="24c12-103">Remove publishedResource from an onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24c12-104">从[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象中删除一个[publishedResource](../resources/publishedresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="24c12-104">Remove a [publishedResource](../resources/publishedresource.md) object from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="24c12-105">权限</span><span class="sxs-lookup"><span data-stu-id="24c12-105">Permissions</span></span>

<span data-ttu-id="24c12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24c12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24c12-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="24c12-108">Permission type</span></span>                        | <span data-ttu-id="24c12-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24c12-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="24c12-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24c12-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="24c12-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="24c12-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="24c12-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24c12-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24c12-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="24c12-113">Not supported.</span></span> |
| <span data-ttu-id="24c12-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="24c12-114">Application</span></span>                            | <span data-ttu-id="24c12-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="24c12-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24c12-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24c12-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="24c12-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="24c12-117">Request headers</span></span>

| <span data-ttu-id="24c12-118">名称</span><span class="sxs-lookup"><span data-stu-id="24c12-118">Name</span></span>          | <span data-ttu-id="24c12-119">说明</span><span class="sxs-lookup"><span data-stu-id="24c12-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="24c12-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="24c12-120">Authorization</span></span> | <span data-ttu-id="24c12-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="24c12-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="24c12-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="24c12-122">Request body</span></span>

<span data-ttu-id="24c12-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="24c12-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24c12-124">响应</span><span class="sxs-lookup"><span data-stu-id="24c12-124">Response</span></span>

<span data-ttu-id="24c12-125">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="24c12-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="24c12-126">示例</span><span class="sxs-lookup"><span data-stu-id="24c12-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24c12-127">请求</span><span class="sxs-lookup"><span data-stu-id="24c12-127">Request</span></span>

<span data-ttu-id="24c12-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="24c12-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="24c12-129">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="24c12-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="24c12-130">C#</span><span class="sxs-lookup"><span data-stu-id="24c12-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onpremisesagentgroup-from-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24c12-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24c12-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="24c12-132">目标-C</span><span class="sxs-lookup"><span data-stu-id="24c12-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="24c12-133">Java</span><span class="sxs-lookup"><span data-stu-id="24c12-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-onpremisesagentgroup-from-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="24c12-134">响应</span><span class="sxs-lookup"><span data-stu-id="24c12-134">Response</span></span>

<span data-ttu-id="24c12-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="24c12-135">The following is an example of the response.</span></span>

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
