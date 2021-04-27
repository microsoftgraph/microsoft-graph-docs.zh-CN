---
title: 将 onPremisesAgent 分配给 onPremisesAgentGroup
description: 将 onPremisesAgent 分配给 onPremisesAgentGroup。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 3ab4e1ed97dec2968bfac63c38d6f2044d4dfc21
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038164"
---
# <a name="assign-onpremisesagent-to-onpremisesagentgroup"></a><span data-ttu-id="488ce-103">将 onPremisesAgent 分配给 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="488ce-103">Assign onPremisesAgent to onPremisesAgentGroup</span></span>

<span data-ttu-id="488ce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="488ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="488ce-105">将 [onPremisesAgent](../resources/onpremisesagent.md) 分配给 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="488ce-105">Assign an [onPremisesAgent](../resources/onpremisesagent.md) to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="488ce-106">权限</span><span class="sxs-lookup"><span data-stu-id="488ce-106">Permissions</span></span>

<span data-ttu-id="488ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="488ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="488ce-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="488ce-109">Permission type</span></span>                        | <span data-ttu-id="488ce-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="488ce-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="488ce-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="488ce-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="488ce-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="488ce-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="488ce-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="488ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="488ce-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="488ce-114">Not supported.</span></span> |
| <span data-ttu-id="488ce-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="488ce-115">Application</span></span>                            | <span data-ttu-id="488ce-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="488ce-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="488ce-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="488ce-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="488ce-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="488ce-118">Request headers</span></span>

| <span data-ttu-id="488ce-119">名称</span><span class="sxs-lookup"><span data-stu-id="488ce-119">Name</span></span>          | <span data-ttu-id="488ce-120">说明</span><span class="sxs-lookup"><span data-stu-id="488ce-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="488ce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="488ce-121">Authorization</span></span> | <span data-ttu-id="488ce-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="488ce-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="488ce-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="488ce-123">Request body</span></span>

<span data-ttu-id="488ce-124">在请求正文中，提供对 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象的 OData 引用的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="488ce-124">In the request body, supply a JSON representation of an OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="488ce-125">响应</span><span class="sxs-lookup"><span data-stu-id="488ce-125">Response</span></span>

<span data-ttu-id="488ce-126">如果成功，此方法在响应正文中返回 响应代码和新的 `201 Created` [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="488ce-126">If successful, this method returns a `201 Created` response code and a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="488ce-127">示例</span><span class="sxs-lookup"><span data-stu-id="488ce-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="488ce-128">请求</span><span class="sxs-lookup"><span data-stu-id="488ce-128">Request</span></span>

<span data-ttu-id="488ce-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="488ce-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="488ce-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="488ce-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisesagent"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
```
# <a name="javascript"></a>[<span data-ttu-id="488ce-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="488ce-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="488ce-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="488ce-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="488ce-133">在请求正文中，提供对 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象的 OData 引用的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="488ce-133">In the request body, supply a JSON representation of OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```http
{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"
}
```

### <a name="response"></a><span data-ttu-id="488ce-134">响应</span><span class="sxs-lookup"><span data-stu-id="488ce-134">Response</span></span>

<span data-ttu-id="488ce-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="488ce-135">The following is an example of the response.</span></span>

> <span data-ttu-id="488ce-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="488ce-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "Create onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



