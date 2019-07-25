---
title: 从 onPremisesAgentGroup 中删除 onpremisesAgent
description: 从 onPremisesAgentGroup 中删除 onpremisesAgent。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46049a549752b27171c7e2e2c8e7c86f51882b73
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878664"
---
# <a name="remove-onpremisesagent-from-an-onpremisesagentgroup"></a><span data-ttu-id="cc697-103">从 onPremisesAgentGroup 中删除 onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="cc697-103">Remove onPremisesAgent from an onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc697-104">从[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)中删除[onPremisesAgent](../resources/onpremisesagent.md) 。</span><span class="sxs-lookup"><span data-stu-id="cc697-104">Remove an [onPremisesAgent](../resources/onpremisesagent.md) from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cc697-105">权限</span><span class="sxs-lookup"><span data-stu-id="cc697-105">Permissions</span></span>

<span data-ttu-id="cc697-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc697-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc697-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc697-108">Permission type</span></span>                        | <span data-ttu-id="cc697-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc697-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc697-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc697-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc697-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="cc697-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="cc697-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc697-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc697-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc697-113">Not supported.</span></span> |
| <span data-ttu-id="cc697-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc697-114">Application</span></span>                            | <span data-ttu-id="cc697-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc697-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc697-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc697-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="cc697-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc697-117">Request headers</span></span>

| <span data-ttu-id="cc697-118">名称</span><span class="sxs-lookup"><span data-stu-id="cc697-118">Name</span></span>          | <span data-ttu-id="cc697-119">说明</span><span class="sxs-lookup"><span data-stu-id="cc697-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cc697-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc697-120">Authorization</span></span> | <span data-ttu-id="cc697-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="cc697-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc697-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc697-122">Request body</span></span>

<span data-ttu-id="cc697-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cc697-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc697-124">响应</span><span class="sxs-lookup"><span data-stu-id="cc697-124">Response</span></span>

<span data-ttu-id="cc697-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cc697-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc697-127">示例</span><span class="sxs-lookup"><span data-stu-id="cc697-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cc697-128">请求</span><span class="sxs-lookup"><span data-stu-id="cc697-128">Request</span></span>

<span data-ttu-id="cc697-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cc697-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cc697-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="cc697-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "Remove onpremisesAgent from an onPremisesAgentGroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cc697-131">C#</span><span class="sxs-lookup"><span data-stu-id="cc697-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/removeonpremisesagentfromanonpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cc697-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="cc697-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/removeonpremisesagentfromanonpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cc697-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="cc697-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/removeonpremisesagentfromanonpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cc697-134">Java</span><span class="sxs-lookup"><span data-stu-id="cc697-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/removeonpremisesagentfromanonpremisesagentgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cc697-135">响应</span><span class="sxs-lookup"><span data-stu-id="cc697-135">Response</span></span>

<span data-ttu-id="cc697-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cc697-136">The following is an example of the response.</span></span>

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
  "description": "Delete onPremisesAgent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
