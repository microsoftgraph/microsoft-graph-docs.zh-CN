---
title: 创建 onPremisesAgentGroup
description: 创建新的 **onPremisesAgentGroup** 对象。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: dab2584a5cb71732fb62352075aae433303e24c4
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781119"
---
# <a name="create-onpremisesagentgroup"></a><span data-ttu-id="6dede-103">创建 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="6dede-103">Create onPremisesAgentGroup</span></span>

<span data-ttu-id="6dede-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dede-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dede-105">创建新的 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6dede-105">Create a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dede-106">权限</span><span class="sxs-lookup"><span data-stu-id="6dede-106">Permissions</span></span>

<span data-ttu-id="6dede-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6dede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6dede-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6dede-109">Permission type</span></span>                        | <span data-ttu-id="6dede-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6dede-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="6dede-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6dede-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6dede-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dede-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="6dede-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6dede-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dede-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dede-114">Not supported.</span></span> |
| <span data-ttu-id="6dede-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6dede-115">Application</span></span>                            | <span data-ttu-id="6dede-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dede-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dede-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6dede-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id}/agents
```

## <a name="request-headers"></a><span data-ttu-id="6dede-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6dede-118">Request headers</span></span>

| <span data-ttu-id="6dede-119">名称</span><span class="sxs-lookup"><span data-stu-id="6dede-119">Name</span></span>          | <span data-ttu-id="6dede-120">说明</span><span class="sxs-lookup"><span data-stu-id="6dede-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6dede-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dede-121">Authorization</span></span> | <span data-ttu-id="6dede-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="6dede-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6dede-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6dede-123">Request body</span></span>

<span data-ttu-id="6dede-124">在请求正文中，提供 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6dede-124">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

## <a name="response"></a><span data-ttu-id="6dede-125">响应</span><span class="sxs-lookup"><span data-stu-id="6dede-125">Response</span></span>

<span data-ttu-id="6dede-126">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6dede-126">If successful, this method returns a `201 Created` response code and an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6dede-127">示例</span><span class="sxs-lookup"><span data-stu-id="6dede-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6dede-128">请求</span><span class="sxs-lookup"><span data-stu-id="6dede-128">Request</span></span>

<span data-ttu-id="6dede-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6dede-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6dede-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dede-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagent_from_onpremisesagentgroup"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups
```
# <a name="javascript"></a>[<span data-ttu-id="6dede-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6dede-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagent-from-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6dede-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6dede-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagent-from-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="6dede-133">在请求正文中，提供 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6dede-133">In the request body, supply a JSON representation of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

### <a name="response"></a><span data-ttu-id="6dede-134">响应</span><span class="sxs-lookup"><span data-stu-id="6dede-134">Response</span></span>

<span data-ttu-id="6dede-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6dede-135">The following is an example of the response.</span></span>

> <span data-ttu-id="6dede-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6dede-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "4655ed41-1619-4848-92bb-0576d3038682",
    "displayName": "New Group",
    "publishingType": "provisioning",
    "isDefault": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create onPremisesAgent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



