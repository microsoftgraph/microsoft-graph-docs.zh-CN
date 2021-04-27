---
title: 创建 featureRolloutPolicy
description: 创建新的 featureRolloutPolicy 对象。
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 020513c2eb1fdc8b05d49b1f34979dcfecf17623
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049917"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="e7990-103">创建 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="e7990-103">Create featureRolloutPolicy</span></span>

<span data-ttu-id="e7990-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7990-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7990-105">创建新的 [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7990-105">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7990-106">权限</span><span class="sxs-lookup"><span data-stu-id="e7990-106">Permissions</span></span>

<span data-ttu-id="e7990-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e7990-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7990-109">Permission type</span></span>                        | <span data-ttu-id="e7990-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e7990-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e7990-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7990-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e7990-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7990-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="e7990-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7990-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7990-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7990-114">Not supported.</span></span> |
| <span data-ttu-id="e7990-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7990-115">Application</span></span>                            | <span data-ttu-id="e7990-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7990-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7990-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7990-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="e7990-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7990-118">Request headers</span></span>

| <span data-ttu-id="e7990-119">名称</span><span class="sxs-lookup"><span data-stu-id="e7990-119">Name</span></span>          | <span data-ttu-id="e7990-120">说明</span><span class="sxs-lookup"><span data-stu-id="e7990-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e7990-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7990-121">Authorization</span></span> | <span data-ttu-id="e7990-122">Bearer {token}。</span><span class="sxs-lookup"><span data-stu-id="e7990-122">Bearer {token}.</span></span> <span data-ttu-id="e7990-123">必需</span><span class="sxs-lookup"><span data-stu-id="e7990-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7990-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7990-124">Request body</span></span>

<span data-ttu-id="e7990-125">在请求正文中，提供 [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7990-125">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="e7990-126">下表显示创建 [featureRolloutPolicy](../resources/featurerolloutpolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e7990-126">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="e7990-127">参数</span><span class="sxs-lookup"><span data-stu-id="e7990-127">Parameter</span></span> | <span data-ttu-id="e7990-128">类型</span><span class="sxs-lookup"><span data-stu-id="e7990-128">Type</span></span> | <span data-ttu-id="e7990-129">说明</span><span class="sxs-lookup"><span data-stu-id="e7990-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7990-130">displayName</span><span class="sxs-lookup"><span data-stu-id="e7990-130">displayName</span></span> |<span data-ttu-id="e7990-131">string</span><span class="sxs-lookup"><span data-stu-id="e7990-131">string</span></span> |<span data-ttu-id="e7990-132">此功能显示名称策略的部署策略。</span><span class="sxs-lookup"><span data-stu-id="e7990-132">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="e7990-133">功能</span><span class="sxs-lookup"><span data-stu-id="e7990-133">feature</span></span> |<span data-ttu-id="e7990-134">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="e7990-134">stagedFeatureName</span></span> |<span data-ttu-id="e7990-135">将使用此策略推出的功能。</span><span class="sxs-lookup"><span data-stu-id="e7990-135">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="e7990-136">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e7990-136">isEnabled</span></span> |<span data-ttu-id="e7990-137">string</span><span class="sxs-lookup"><span data-stu-id="e7990-137">string</span></span> |<span data-ttu-id="e7990-138">指示是否启用功能推出。</span><span class="sxs-lookup"><span data-stu-id="e7990-138">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="e7990-139">响应</span><span class="sxs-lookup"><span data-stu-id="e7990-139">Response</span></span>

<span data-ttu-id="e7990-140">如果成功，此方法在响应正文中返回 响应代码和一 `201 Created` 个新的 [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7990-140">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e7990-141">示例</span><span class="sxs-lookup"><span data-stu-id="e7990-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e7990-142">请求</span><span class="sxs-lookup"><span data-stu-id="e7990-142">Request</span></span>

<span data-ttu-id="e7990-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e7990-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e7990-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7990-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_featurerolloutpolicy_from_policies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/featureRolloutPolicies
Content-type: application/json

{
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```
# <a name="c"></a>[<span data-ttu-id="e7990-145">C#</span><span class="sxs-lookup"><span data-stu-id="e7990-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-featurerolloutpolicy-from-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7990-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7990-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-featurerolloutpolicy-from-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7990-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7990-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-featurerolloutpolicy-from-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7990-148">Java</span><span class="sxs-lookup"><span data-stu-id="e7990-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-featurerolloutpolicy-from-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e7990-149">响应</span><span class="sxs-lookup"><span data-stu-id="e7990-149">Response</span></span>

<span data-ttu-id="e7990-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e7990-150">The following is an example of the response.</span></span>

> <span data-ttu-id="e7990-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e7990-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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


