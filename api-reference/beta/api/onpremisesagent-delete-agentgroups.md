---
title: 从 onPremisesAgentGroup 中删除 onpremisesAgent
description: 从 onPremisesAgentGroup 中删除 onpremisesAgent。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 76462a4b998f29db1eb43b3cca2618b1db4b4fa2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456514"
---
# <a name="remove-onpremisesagent-from-an-onpremisesagentgroup"></a><span data-ttu-id="6f176-103">从 onPremisesAgentGroup 中删除 onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="6f176-103">Remove onPremisesAgent from an onPremisesAgentGroup</span></span>

<span data-ttu-id="6f176-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6f176-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f176-105">从[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)中删除[onPremisesAgent](../resources/onpremisesagent.md) 。</span><span class="sxs-lookup"><span data-stu-id="6f176-105">Remove an [onPremisesAgent](../resources/onpremisesagent.md) from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6f176-106">权限</span><span class="sxs-lookup"><span data-stu-id="6f176-106">Permissions</span></span>

<span data-ttu-id="6f176-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f176-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6f176-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f176-109">Permission type</span></span>                        | <span data-ttu-id="6f176-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f176-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f176-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f176-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f176-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f176-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="6f176-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f176-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f176-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f176-114">Not supported.</span></span> |
| <span data-ttu-id="6f176-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f176-115">Application</span></span>                            | <span data-ttu-id="6f176-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f176-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f176-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f176-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6f176-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f176-118">Request headers</span></span>

| <span data-ttu-id="6f176-119">名称</span><span class="sxs-lookup"><span data-stu-id="6f176-119">Name</span></span>          | <span data-ttu-id="6f176-120">说明</span><span class="sxs-lookup"><span data-stu-id="6f176-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6f176-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f176-121">Authorization</span></span> | <span data-ttu-id="6f176-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="6f176-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f176-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f176-123">Request body</span></span>

<span data-ttu-id="6f176-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6f176-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f176-125">响应</span><span class="sxs-lookup"><span data-stu-id="6f176-125">Response</span></span>

<span data-ttu-id="6f176-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6f176-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f176-128">示例</span><span class="sxs-lookup"><span data-stu-id="6f176-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6f176-129">请求</span><span class="sxs-lookup"><span data-stu-id="6f176-129">Request</span></span>

<span data-ttu-id="6f176-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6f176-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6f176-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f176-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "Remove onpremisesAgent from an onPremisesAgentGroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="6f176-132">C#</span><span class="sxs-lookup"><span data-stu-id="6f176-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/removeonpremisesagentfromanonpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f176-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f176-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/removeonpremisesagentfromanonpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f176-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f176-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/removeonpremisesagentfromanonpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6f176-135">响应</span><span class="sxs-lookup"><span data-stu-id="6f176-135">Response</span></span>

<span data-ttu-id="6f176-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6f176-136">The following is an example of the response.</span></span>

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
