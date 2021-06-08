---
title: 将 onPremisesAgent 分配给 onPremisesAgentGroup
description: 将 onPremisesAgent 分配给 onPremisesAgentGroup。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 9788e4485ba5c81453aac5087661bf3ea3e98299
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787537"
---
# <a name="assign-onpremisesagent-to-onpremisesagentgroup"></a><span data-ttu-id="cae98-103">将 onPremisesAgent 分配给 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="cae98-103">Assign onPremisesAgent to onPremisesAgentGroup</span></span>

<span data-ttu-id="cae98-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cae98-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cae98-105">将 [onPremisesAgent](../resources/onpremisesagent.md) 分配给 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cae98-105">Assign an [onPremisesAgent](../resources/onpremisesagent.md) to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cae98-106">权限</span><span class="sxs-lookup"><span data-stu-id="cae98-106">Permissions</span></span>

<span data-ttu-id="cae98-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cae98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cae98-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cae98-109">Permission type</span></span>                        | <span data-ttu-id="cae98-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cae98-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="cae98-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cae98-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cae98-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cae98-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="cae98-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cae98-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cae98-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cae98-114">Not supported.</span></span> |
| <span data-ttu-id="cae98-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cae98-115">Application</span></span>                            | <span data-ttu-id="cae98-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cae98-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cae98-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cae98-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="cae98-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cae98-118">Request headers</span></span>

| <span data-ttu-id="cae98-119">名称</span><span class="sxs-lookup"><span data-stu-id="cae98-119">Name</span></span>          | <span data-ttu-id="cae98-120">说明</span><span class="sxs-lookup"><span data-stu-id="cae98-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cae98-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cae98-121">Authorization</span></span> | <span data-ttu-id="cae98-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="cae98-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cae98-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="cae98-123">Request body</span></span>

<span data-ttu-id="cae98-124">在请求正文中，提供对 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象的 OData 引用的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cae98-124">In the request body, supply a JSON representation of an OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cae98-125">响应</span><span class="sxs-lookup"><span data-stu-id="cae98-125">Response</span></span>

<span data-ttu-id="cae98-126">如果成功，此方法在响应正文中返回 响应代码和新的 `201 Created` [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cae98-126">If successful, this method returns a `201 Created` response code and a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cae98-127">示例</span><span class="sxs-lookup"><span data-stu-id="cae98-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cae98-128">请求</span><span class="sxs-lookup"><span data-stu-id="cae98-128">Request</span></span>

<span data-ttu-id="cae98-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cae98-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cae98-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="cae98-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisesagent"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
```
# <a name="javascript"></a>[<span data-ttu-id="cae98-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cae98-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cae98-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cae98-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="cae98-133">在请求正文中，提供对 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象的 OData 引用的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cae98-133">In the request body, supply a JSON representation of OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```http
{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"
}
```

### <a name="response"></a><span data-ttu-id="cae98-134">响应</span><span class="sxs-lookup"><span data-stu-id="cae98-134">Response</span></span>

<span data-ttu-id="cae98-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cae98-135">The following is an example of the response.</span></span>

> <span data-ttu-id="cae98-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cae98-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "Create onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



