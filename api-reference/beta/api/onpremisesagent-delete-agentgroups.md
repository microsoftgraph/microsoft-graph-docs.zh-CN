---
title: 从 onPremisesAgentGroup 中删除 onpremisesAgent
description: 从 onPremisesAgentGroup 中删除 onpremisesAgent。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 41719b5431bf04759788b56973a2dc11c5113b71
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136484"
---
# <a name="remove-onpremisesagent-from-an-onpremisesagentgroup"></a><span data-ttu-id="a1f14-103">从 onPremisesAgentGroup 中删除 onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="a1f14-103">Remove onPremisesAgent from an onPremisesAgentGroup</span></span>

<span data-ttu-id="a1f14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1f14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1f14-105">从 [onPremisesAgentGroup](../resources/onpremisesagent.md) 中删除 [onPremisesAgent](../resources/onpremisesagentgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="a1f14-105">Remove an [onPremisesAgent](../resources/onpremisesagent.md) from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a1f14-106">权限</span><span class="sxs-lookup"><span data-stu-id="a1f14-106">Permissions</span></span>

<span data-ttu-id="a1f14-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1f14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1f14-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1f14-109">Permission type</span></span>                        | <span data-ttu-id="a1f14-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1f14-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1f14-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1f14-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1f14-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1f14-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="a1f14-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1f14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1f14-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1f14-114">Not supported.</span></span> |
| <span data-ttu-id="a1f14-115">Application</span><span class="sxs-lookup"><span data-stu-id="a1f14-115">Application</span></span>                            | <span data-ttu-id="a1f14-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1f14-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1f14-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1f14-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a1f14-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1f14-118">Request headers</span></span>

| <span data-ttu-id="a1f14-119">名称</span><span class="sxs-lookup"><span data-stu-id="a1f14-119">Name</span></span>          | <span data-ttu-id="a1f14-120">说明</span><span class="sxs-lookup"><span data-stu-id="a1f14-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a1f14-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1f14-121">Authorization</span></span> | <span data-ttu-id="a1f14-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="a1f14-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1f14-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1f14-123">Request body</span></span>

<span data-ttu-id="a1f14-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1f14-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1f14-125">响应</span><span class="sxs-lookup"><span data-stu-id="a1f14-125">Response</span></span>

<span data-ttu-id="a1f14-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a1f14-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a1f14-128">示例</span><span class="sxs-lookup"><span data-stu-id="a1f14-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a1f14-129">请求</span><span class="sxs-lookup"><span data-stu-id="a1f14-129">Request</span></span>

<span data-ttu-id="a1f14-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a1f14-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1f14-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1f14-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "Remove onpremisesAgent from an onPremisesAgentGroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="a1f14-132">C#</span><span class="sxs-lookup"><span data-stu-id="a1f14-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/removeonpremisesagentfromanonpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1f14-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1f14-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/removeonpremisesagentfromanonpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1f14-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1f14-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/removeonpremisesagentfromanonpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a1f14-135">Java</span><span class="sxs-lookup"><span data-stu-id="a1f14-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/removeonpremisesagentfromanonpremisesagentgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a1f14-136">响应</span><span class="sxs-lookup"><span data-stu-id="a1f14-136">Response</span></span>

<span data-ttu-id="a1f14-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a1f14-137">The following is an example of the response.</span></span>

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



