---
title: 将 onPremisesAgent 分配给 onPremisesAgentGroup
description: 将 onPremisesAgent 分配给 onPremisesAgentGroup。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 000385e1b2faad98bee217d2709f5516ea40b6b6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342640"
---
# <a name="assign-onpremisesagent-to-onpremisesagentgroup"></a><span data-ttu-id="fd5f5-103">将 onPremisesAgent 分配给 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="fd5f5-103">Assign onPremisesAgent to onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd5f5-104">将[onPremisesAgent](../resources/onpremisesagent.md)分配给[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fd5f5-104">Assign an [onPremisesAgent](../resources/onpremisesagent.md) to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd5f5-105">权限</span><span class="sxs-lookup"><span data-stu-id="fd5f5-105">Permissions</span></span>

<span data-ttu-id="fd5f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fd5f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fd5f5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd5f5-108">Permission type</span></span>                        | <span data-ttu-id="fd5f5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fd5f5-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd5f5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd5f5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fd5f5-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="fd5f5-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="fd5f5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd5f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd5f5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd5f5-113">Not supported.</span></span> |
| <span data-ttu-id="fd5f5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd5f5-114">Application</span></span>                            | <span data-ttu-id="fd5f5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd5f5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd5f5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd5f5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="fd5f5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd5f5-117">Request headers</span></span>

| <span data-ttu-id="fd5f5-118">名称</span><span class="sxs-lookup"><span data-stu-id="fd5f5-118">Name</span></span>          | <span data-ttu-id="fd5f5-119">说明</span><span class="sxs-lookup"><span data-stu-id="fd5f5-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fd5f5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd5f5-120">Authorization</span></span> | <span data-ttu-id="fd5f5-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="fd5f5-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd5f5-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd5f5-122">Request body</span></span>

<span data-ttu-id="fd5f5-123">在请求正文中, 提供对[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象的 OData 引用的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd5f5-123">In the request body, supply a JSON representation of an OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fd5f5-124">响应</span><span class="sxs-lookup"><span data-stu-id="fd5f5-124">Response</span></span>

<span data-ttu-id="fd5f5-125">如果成功, 此方法在响应`201 Created`正文中返回响应代码和新的[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fd5f5-125">If successful, this method returns a `201 Created` response code and a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fd5f5-126">示例</span><span class="sxs-lookup"><span data-stu-id="fd5f5-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fd5f5-127">请求</span><span class="sxs-lookup"><span data-stu-id="fd5f5-127">Request</span></span>

<span data-ttu-id="fd5f5-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fd5f5-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fd5f5-129">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fd5f5-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisesagent"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd5f5-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd5f5-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fd5f5-131">目标-C</span><span class="sxs-lookup"><span data-stu-id="fd5f5-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="fd5f5-132">在请求正文中, 提供对[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象的 OData 引用的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd5f5-132">In the request body, supply a JSON representation of OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```http
{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"
}
```

### <a name="response"></a><span data-ttu-id="fd5f5-133">响应</span><span class="sxs-lookup"><span data-stu-id="fd5f5-133">Response</span></span>

<span data-ttu-id="fd5f5-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fd5f5-134">The following is an example of the response.</span></span>

> <span data-ttu-id="fd5f5-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fd5f5-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
