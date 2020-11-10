---
title: 更新 onPremisesAgentGroup
description: 更新 **onPremisesAgentGroup** 对象的属性。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 08a2816e21c69ccb1b8104faef829b0d806d8cc0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976901"
---
# <a name="update-onpremisesagentgroup"></a><span data-ttu-id="9d72e-103">更新 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="9d72e-103">Update onPremisesAgentGroup</span></span>

<span data-ttu-id="9d72e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d72e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d72e-105">更新 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9d72e-105">Update the properties of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d72e-106">权限</span><span class="sxs-lookup"><span data-stu-id="9d72e-106">Permissions</span></span>

<span data-ttu-id="9d72e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d72e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d72e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d72e-109">Permission type</span></span>                        | <span data-ttu-id="9d72e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d72e-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d72e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d72e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d72e-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d72e-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="9d72e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d72e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d72e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d72e-114">Not supported.</span></span> |
| <span data-ttu-id="9d72e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d72e-115">Application</span></span>                            | <span data-ttu-id="9d72e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d72e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d72e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d72e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="request-headers"></a><span data-ttu-id="9d72e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d72e-118">Request headers</span></span>

| <span data-ttu-id="9d72e-119">名称</span><span class="sxs-lookup"><span data-stu-id="9d72e-119">Name</span></span>       | <span data-ttu-id="9d72e-120">说明</span><span class="sxs-lookup"><span data-stu-id="9d72e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9d72e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d72e-121">Authorization</span></span> | <span data-ttu-id="9d72e-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9d72e-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d72e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d72e-123">Request body</span></span>

<span data-ttu-id="9d72e-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="9d72e-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9d72e-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="9d72e-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9d72e-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9d72e-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="9d72e-127">以下是您可以更新的属性的列表。</span><span class="sxs-lookup"><span data-stu-id="9d72e-127">The following is the list of properties that you can update.</span></span>

| <span data-ttu-id="9d72e-128">属性</span><span class="sxs-lookup"><span data-stu-id="9d72e-128">Property</span></span>     | <span data-ttu-id="9d72e-129">类型</span><span class="sxs-lookup"><span data-stu-id="9d72e-129">Type</span></span>        | <span data-ttu-id="9d72e-130">说明</span><span class="sxs-lookup"><span data-stu-id="9d72e-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9d72e-131">displayName</span><span class="sxs-lookup"><span data-stu-id="9d72e-131">displayName</span></span>|<span data-ttu-id="9d72e-132">String</span><span class="sxs-lookup"><span data-stu-id="9d72e-132">String</span></span>| <span data-ttu-id="9d72e-133">表示内部部署代理组名称。</span><span class="sxs-lookup"><span data-stu-id="9d72e-133">Represents the on-premises agents group name.</span></span>|

## <a name="response"></a><span data-ttu-id="9d72e-134">响应</span><span class="sxs-lookup"><span data-stu-id="9d72e-134">Response</span></span>

<span data-ttu-id="9d72e-135">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9d72e-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9d72e-136">示例</span><span class="sxs-lookup"><span data-stu-id="9d72e-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9d72e-137">请求</span><span class="sxs-lookup"><span data-stu-id="9d72e-137">Request</span></span>

<span data-ttu-id="9d72e-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9d72e-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9d72e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d72e-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_onpremisesagentgroup"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/
Content-type: application/json

{
    "displayName": "Group New Name"
}
```
# <a name="c"></a>[<span data-ttu-id="9d72e-140">C#</span><span class="sxs-lookup"><span data-stu-id="9d72e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d72e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d72e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d72e-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d72e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d72e-143">Java</span><span class="sxs-lookup"><span data-stu-id="9d72e-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisesagentgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9d72e-144">响应</span><span class="sxs-lookup"><span data-stu-id="9d72e-144">Response</span></span>

<span data-ttu-id="9d72e-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9d72e-145">The following is an example of the response.</span></span>

> <span data-ttu-id="9d72e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9d72e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Update onpremisesagentgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


