---
title: 创建 featureRolloutPolicy
description: 创建新的 featureRolloutPolicy 对象。
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8d7d670303748893fdb7e5825369861dea502178
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963213"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="be0d3-103">创建 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="be0d3-103">Create featureRolloutPolicy</span></span>

<span data-ttu-id="be0d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be0d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be0d3-105">创建新的 [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be0d3-105">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be0d3-106">权限</span><span class="sxs-lookup"><span data-stu-id="be0d3-106">Permissions</span></span>

<span data-ttu-id="be0d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be0d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be0d3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="be0d3-109">Permission type</span></span>                        | <span data-ttu-id="be0d3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be0d3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be0d3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be0d3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be0d3-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="be0d3-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="be0d3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be0d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be0d3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="be0d3-114">Not supported.</span></span> |
| <span data-ttu-id="be0d3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="be0d3-115">Application</span></span>                            | <span data-ttu-id="be0d3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="be0d3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be0d3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be0d3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="be0d3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="be0d3-118">Request headers</span></span>

| <span data-ttu-id="be0d3-119">名称</span><span class="sxs-lookup"><span data-stu-id="be0d3-119">Name</span></span>          | <span data-ttu-id="be0d3-120">说明</span><span class="sxs-lookup"><span data-stu-id="be0d3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="be0d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="be0d3-121">Authorization</span></span> | <span data-ttu-id="be0d3-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="be0d3-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="be0d3-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="be0d3-123">Request body</span></span>

<span data-ttu-id="be0d3-124">在请求正文中，提供 [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be0d3-124">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="be0d3-125">下表显示创建 [featureRolloutPolicy](../resources/featurerolloutpolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="be0d3-125">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="be0d3-126">参数</span><span class="sxs-lookup"><span data-stu-id="be0d3-126">Parameter</span></span> | <span data-ttu-id="be0d3-127">类型</span><span class="sxs-lookup"><span data-stu-id="be0d3-127">Type</span></span> | <span data-ttu-id="be0d3-128">说明</span><span class="sxs-lookup"><span data-stu-id="be0d3-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be0d3-129">displayName</span><span class="sxs-lookup"><span data-stu-id="be0d3-129">displayName</span></span> |<span data-ttu-id="be0d3-130">string</span><span class="sxs-lookup"><span data-stu-id="be0d3-130">string</span></span> |<span data-ttu-id="be0d3-131">此功能展示策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="be0d3-131">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="be0d3-132">功能</span><span class="sxs-lookup"><span data-stu-id="be0d3-132">feature</span></span> |<span data-ttu-id="be0d3-133">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="be0d3-133">stagedFeatureName</span></span> |<span data-ttu-id="be0d3-134">将使用此策略进行推出的功能。</span><span class="sxs-lookup"><span data-stu-id="be0d3-134">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="be0d3-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="be0d3-135">isEnabled</span></span> |<span data-ttu-id="be0d3-136">string</span><span class="sxs-lookup"><span data-stu-id="be0d3-136">string</span></span> |<span data-ttu-id="be0d3-137">指示是否启用功能展示。</span><span class="sxs-lookup"><span data-stu-id="be0d3-137">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="be0d3-138">响应</span><span class="sxs-lookup"><span data-stu-id="be0d3-138">Response</span></span>

<span data-ttu-id="be0d3-139">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be0d3-139">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be0d3-140">示例</span><span class="sxs-lookup"><span data-stu-id="be0d3-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be0d3-141">请求</span><span class="sxs-lookup"><span data-stu-id="be0d3-141">Request</span></span>

<span data-ttu-id="be0d3-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="be0d3-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="be0d3-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="be0d3-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_featurerolloutpolicy_from_directory"
}-->

```http
POST https://graph.microsoft.com/beta/directory/featureRolloutPolicies
Content-type: application/json

{
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```
# <a name="c"></a>[<span data-ttu-id="be0d3-144">C#</span><span class="sxs-lookup"><span data-stu-id="be0d3-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-featurerolloutpolicy-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be0d3-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be0d3-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-featurerolloutpolicy-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be0d3-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be0d3-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-featurerolloutpolicy-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="be0d3-147">Java</span><span class="sxs-lookup"><span data-stu-id="be0d3-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-featurerolloutpolicy-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="be0d3-148">响应</span><span class="sxs-lookup"><span data-stu-id="be0d3-148">Response</span></span>

<span data-ttu-id="be0d3-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="be0d3-149">The following is an example of the response.</span></span>

> <span data-ttu-id="be0d3-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="be0d3-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "e3c2f23a-edd2-43a8-849f-154e70794ac5",
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


