---
title: 更新 onPremisesAgentGroup
description: 更新 **onPremisesAgentGroup** 对象的属性。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1d2aac32242617891574e2aa51f220e8d990e7e1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010778"
---
# <a name="update-onpremisesagentgroup"></a><span data-ttu-id="c1a14-103">更新 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="c1a14-103">Update onPremisesAgentGroup</span></span>

<span data-ttu-id="c1a14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1a14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1a14-105">更新 [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c1a14-105">Update the properties of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1a14-106">权限</span><span class="sxs-lookup"><span data-stu-id="c1a14-106">Permissions</span></span>

<span data-ttu-id="c1a14-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1a14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1a14-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1a14-109">Permission type</span></span>                        | <span data-ttu-id="c1a14-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1a14-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1a14-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1a14-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1a14-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1a14-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="c1a14-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1a14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1a14-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1a14-114">Not supported.</span></span> |
| <span data-ttu-id="c1a14-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1a14-115">Application</span></span>                            | <span data-ttu-id="c1a14-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1a14-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1a14-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1a14-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="request-headers"></a><span data-ttu-id="c1a14-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1a14-118">Request headers</span></span>

| <span data-ttu-id="c1a14-119">名称</span><span class="sxs-lookup"><span data-stu-id="c1a14-119">Name</span></span>       | <span data-ttu-id="c1a14-120">说明</span><span class="sxs-lookup"><span data-stu-id="c1a14-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c1a14-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1a14-121">Authorization</span></span> | <span data-ttu-id="c1a14-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="c1a14-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1a14-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1a14-123">Request body</span></span>

<span data-ttu-id="c1a14-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="c1a14-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c1a14-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="c1a14-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c1a14-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c1a14-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="c1a14-127">以下是您可以更新的属性的列表。</span><span class="sxs-lookup"><span data-stu-id="c1a14-127">The following is the list of properties that you can update.</span></span>

| <span data-ttu-id="c1a14-128">属性</span><span class="sxs-lookup"><span data-stu-id="c1a14-128">Property</span></span>     | <span data-ttu-id="c1a14-129">类型</span><span class="sxs-lookup"><span data-stu-id="c1a14-129">Type</span></span>        | <span data-ttu-id="c1a14-130">说明</span><span class="sxs-lookup"><span data-stu-id="c1a14-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c1a14-131">displayName</span><span class="sxs-lookup"><span data-stu-id="c1a14-131">displayName</span></span>|<span data-ttu-id="c1a14-132">String</span><span class="sxs-lookup"><span data-stu-id="c1a14-132">String</span></span>| <span data-ttu-id="c1a14-133">表示内部部署代理组名称。</span><span class="sxs-lookup"><span data-stu-id="c1a14-133">Represents the on-premises agents group name.</span></span>|

## <a name="response"></a><span data-ttu-id="c1a14-134">响应</span><span class="sxs-lookup"><span data-stu-id="c1a14-134">Response</span></span>

<span data-ttu-id="c1a14-135">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c1a14-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c1a14-136">示例</span><span class="sxs-lookup"><span data-stu-id="c1a14-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c1a14-137">请求</span><span class="sxs-lookup"><span data-stu-id="c1a14-137">Request</span></span>

<span data-ttu-id="c1a14-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1a14-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c1a14-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1a14-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c1a14-140">C#</span><span class="sxs-lookup"><span data-stu-id="c1a14-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1a14-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1a14-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1a14-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1a14-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c1a14-143">响应</span><span class="sxs-lookup"><span data-stu-id="c1a14-143">Response</span></span>

<span data-ttu-id="c1a14-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1a14-144">The following is an example of the response.</span></span>

> <span data-ttu-id="c1a14-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c1a14-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


