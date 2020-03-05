---
title: 将 onPremisesAgent 分配给 onPremisesAgentGroup
description: 将 onPremisesAgent 分配给 onPremisesAgentGroup。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a1f2f3df53414f7f042a444d0482f50c51246e3f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456486"
---
# <a name="assign-onpremisesagent-to-onpremisesagentgroup"></a><span data-ttu-id="5e64a-103">将 onPremisesAgent 分配给 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="5e64a-103">Assign onPremisesAgent to onPremisesAgentGroup</span></span>

<span data-ttu-id="5e64a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5e64a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e64a-105">将[onPremisesAgent](../resources/onpremisesagent.md)分配给[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5e64a-105">Assign an [onPremisesAgent](../resources/onpremisesagent.md) to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e64a-106">权限</span><span class="sxs-lookup"><span data-stu-id="5e64a-106">Permissions</span></span>

<span data-ttu-id="5e64a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e64a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e64a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e64a-109">Permission type</span></span>                        | <span data-ttu-id="5e64a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e64a-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e64a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e64a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5e64a-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e64a-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="5e64a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e64a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e64a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e64a-114">Not supported.</span></span> |
| <span data-ttu-id="5e64a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e64a-115">Application</span></span>                            | <span data-ttu-id="5e64a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e64a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e64a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e64a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5e64a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e64a-118">Request headers</span></span>

| <span data-ttu-id="5e64a-119">名称</span><span class="sxs-lookup"><span data-stu-id="5e64a-119">Name</span></span>          | <span data-ttu-id="5e64a-120">说明</span><span class="sxs-lookup"><span data-stu-id="5e64a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5e64a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e64a-121">Authorization</span></span> | <span data-ttu-id="5e64a-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="5e64a-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e64a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e64a-123">Request body</span></span>

<span data-ttu-id="5e64a-124">在请求正文中，提供对[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象的 OData 引用的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e64a-124">In the request body, supply a JSON representation of an OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5e64a-125">响应</span><span class="sxs-lookup"><span data-stu-id="5e64a-125">Response</span></span>

<span data-ttu-id="5e64a-126">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5e64a-126">If successful, this method returns a `201 Created` response code and a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5e64a-127">示例</span><span class="sxs-lookup"><span data-stu-id="5e64a-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5e64a-128">请求</span><span class="sxs-lookup"><span data-stu-id="5e64a-128">Request</span></span>

<span data-ttu-id="5e64a-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5e64a-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e64a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e64a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisesagent"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
```
# <a name="javascript"></a>[<span data-ttu-id="5e64a-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e64a-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e64a-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e64a-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="5e64a-133">在请求正文中，提供对[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象的 OData 引用的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e64a-133">In the request body, supply a JSON representation of OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```http
{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"
}
```

### <a name="response"></a><span data-ttu-id="5e64a-134">响应</span><span class="sxs-lookup"><span data-stu-id="5e64a-134">Response</span></span>

<span data-ttu-id="5e64a-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5e64a-135">The following is an example of the response.</span></span>

> <span data-ttu-id="5e64a-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5e64a-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
