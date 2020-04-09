---
title: 创建 onPremisesAgentGroup
description: 创建新的**onPremisesAgentGroup**对象。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1dfce148cd74d01bd838b4d30c40cac8af145f35
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200276"
---
# <a name="create-onpremisesagentgroup"></a><span data-ttu-id="d05a0-103">创建 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="d05a0-103">Create onPremisesAgentGroup</span></span>

<span data-ttu-id="d05a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d05a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d05a0-105">创建新的[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d05a0-105">Create a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d05a0-106">权限</span><span class="sxs-lookup"><span data-stu-id="d05a0-106">Permissions</span></span>

<span data-ttu-id="d05a0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d05a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d05a0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d05a0-109">Permission type</span></span>                        | <span data-ttu-id="d05a0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d05a0-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d05a0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d05a0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d05a0-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d05a0-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="d05a0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d05a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d05a0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d05a0-114">Not supported.</span></span> |
| <span data-ttu-id="d05a0-115">Application</span><span class="sxs-lookup"><span data-stu-id="d05a0-115">Application</span></span>                            | <span data-ttu-id="d05a0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d05a0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d05a0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d05a0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id}/agents
```

## <a name="request-headers"></a><span data-ttu-id="d05a0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d05a0-118">Request headers</span></span>

| <span data-ttu-id="d05a0-119">名称</span><span class="sxs-lookup"><span data-stu-id="d05a0-119">Name</span></span>          | <span data-ttu-id="d05a0-120">说明</span><span class="sxs-lookup"><span data-stu-id="d05a0-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d05a0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d05a0-121">Authorization</span></span> | <span data-ttu-id="d05a0-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d05a0-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d05a0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d05a0-123">Request body</span></span>

<span data-ttu-id="d05a0-124">在请求正文中，提供[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d05a0-124">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

## <a name="response"></a><span data-ttu-id="d05a0-125">响应</span><span class="sxs-lookup"><span data-stu-id="d05a0-125">Response</span></span>

<span data-ttu-id="d05a0-126">如果成功，此方法在响应`201 Created`正文中返回响应代码和[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d05a0-126">If successful, this method returns a `201 Created` response code and an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d05a0-127">示例</span><span class="sxs-lookup"><span data-stu-id="d05a0-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d05a0-128">请求</span><span class="sxs-lookup"><span data-stu-id="d05a0-128">Request</span></span>

<span data-ttu-id="d05a0-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d05a0-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d05a0-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d05a0-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagent_from_onpremisesagentgroup"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups
```
# <a name="javascript"></a>[<span data-ttu-id="d05a0-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d05a0-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagent-from-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d05a0-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d05a0-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagent-from-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="d05a0-133">在请求正文中，提供[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d05a0-133">In the request body, supply a JSON representation of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

### <a name="response"></a><span data-ttu-id="d05a0-134">响应</span><span class="sxs-lookup"><span data-stu-id="d05a0-134">Response</span></span>

<span data-ttu-id="d05a0-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d05a0-135">The following is an example of the response.</span></span>

> <span data-ttu-id="d05a0-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d05a0-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
