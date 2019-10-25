---
title: 从 onPremisesAgentGroup 中删除 onpremisesAgent
description: 从 onPremisesAgentGroup 中删除 onpremisesAgent。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7e8fbd52349ef7009c00e268d76c9867b50b5194
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/25/2019
ms.locfileid: "37726392"
---
# <a name="remove-onpremisesagent-from-an-onpremisesagentgroup"></a><span data-ttu-id="a9dcd-103">从 onPremisesAgentGroup 中删除 onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="a9dcd-103">Remove onPremisesAgent from an onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9dcd-104">从[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)中删除[onPremisesAgent](../resources/onpremisesagent.md) 。</span><span class="sxs-lookup"><span data-stu-id="a9dcd-104">Remove an [onPremisesAgent](../resources/onpremisesagent.md) from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a9dcd-105">权限</span><span class="sxs-lookup"><span data-stu-id="a9dcd-105">Permissions</span></span>

<span data-ttu-id="a9dcd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9dcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9dcd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9dcd-108">Permission type</span></span>                        | <span data-ttu-id="a9dcd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9dcd-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9dcd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9dcd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9dcd-111">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9dcd-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="a9dcd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9dcd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9dcd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9dcd-113">Not supported.</span></span> |
| <span data-ttu-id="a9dcd-114">Application</span><span class="sxs-lookup"><span data-stu-id="a9dcd-114">Application</span></span>                            | <span data-ttu-id="a9dcd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9dcd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9dcd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9dcd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a9dcd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9dcd-117">Request headers</span></span>

| <span data-ttu-id="a9dcd-118">名称</span><span class="sxs-lookup"><span data-stu-id="a9dcd-118">Name</span></span>          | <span data-ttu-id="a9dcd-119">说明</span><span class="sxs-lookup"><span data-stu-id="a9dcd-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a9dcd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9dcd-120">Authorization</span></span> | <span data-ttu-id="a9dcd-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="a9dcd-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9dcd-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9dcd-122">Request body</span></span>

<span data-ttu-id="a9dcd-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a9dcd-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9dcd-124">响应</span><span class="sxs-lookup"><span data-stu-id="a9dcd-124">Response</span></span>

<span data-ttu-id="a9dcd-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a9dcd-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9dcd-127">示例</span><span class="sxs-lookup"><span data-stu-id="a9dcd-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a9dcd-128">请求</span><span class="sxs-lookup"><span data-stu-id="a9dcd-128">Request</span></span>

<span data-ttu-id="a9dcd-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a9dcd-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a9dcd-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9dcd-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "Remove onpremisesAgent from an onPremisesAgentGroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a9dcd-131">C#</span><span class="sxs-lookup"><span data-stu-id="a9dcd-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/removeonpremisesagentfromanonpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9dcd-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9dcd-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/removeonpremisesagentfromanonpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a9dcd-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9dcd-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/removeonpremisesagentfromanonpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a9dcd-134">响应</span><span class="sxs-lookup"><span data-stu-id="a9dcd-134">Response</span></span>

<span data-ttu-id="a9dcd-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a9dcd-135">The following is an example of the response.</span></span>

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
