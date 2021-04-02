---
title: 更新 featureRolloutPolicy
description: 更新 featurerolloutpolicy 对象的属性。
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8d30e3df9d807289787f599e436427a02544c055
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508595"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="0e31a-103">更新 featurerolloutpolicy</span><span class="sxs-lookup"><span data-stu-id="0e31a-103">Update featurerolloutpolicy</span></span>

<span data-ttu-id="0e31a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e31a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e31a-105">更新 [featureRolloutPolicy 对象](../resources/featurerolloutpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="0e31a-105">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e31a-106">权限</span><span class="sxs-lookup"><span data-stu-id="0e31a-106">Permissions</span></span>

<span data-ttu-id="0e31a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e31a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e31a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e31a-109">Permission type</span></span>                        | <span data-ttu-id="0e31a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e31a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0e31a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e31a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e31a-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e31a-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="0e31a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e31a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e31a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e31a-114">Not supported.</span></span> |
| <span data-ttu-id="0e31a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e31a-115">Application</span></span>                            | <span data-ttu-id="0e31a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e31a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e31a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e31a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0e31a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e31a-118">Request headers</span></span>

| <span data-ttu-id="0e31a-119">名称</span><span class="sxs-lookup"><span data-stu-id="0e31a-119">Name</span></span>       | <span data-ttu-id="0e31a-120">说明</span><span class="sxs-lookup"><span data-stu-id="0e31a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0e31a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e31a-121">Authorization</span></span> | <span data-ttu-id="0e31a-122">Bearer {token}。</span><span class="sxs-lookup"><span data-stu-id="0e31a-122">Bearer {token}.</span></span> <span data-ttu-id="0e31a-123">必需</span><span class="sxs-lookup"><span data-stu-id="0e31a-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e31a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e31a-124">Request body</span></span>

<span data-ttu-id="0e31a-125">在请求正文中，提供应更新的相关属性的值。</span><span class="sxs-lookup"><span data-stu-id="0e31a-125">In the request body, supply the values for relevant properties that should be updated.</span></span> <span data-ttu-id="0e31a-126">未添加到请求正文的现有属性要么保留旧值，要么根据其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="0e31a-126">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="0e31a-127">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0e31a-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0e31a-128">属性</span><span class="sxs-lookup"><span data-stu-id="0e31a-128">Property</span></span>     | <span data-ttu-id="0e31a-129">类型</span><span class="sxs-lookup"><span data-stu-id="0e31a-129">Type</span></span>        | <span data-ttu-id="0e31a-130">说明</span><span class="sxs-lookup"><span data-stu-id="0e31a-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0e31a-131">说明</span><span class="sxs-lookup"><span data-stu-id="0e31a-131">description</span></span>|<span data-ttu-id="0e31a-132">字符串</span><span class="sxs-lookup"><span data-stu-id="0e31a-132">String</span></span>|<span data-ttu-id="0e31a-133">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="0e31a-133">A description for this policy.</span></span>|
|<span data-ttu-id="0e31a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="0e31a-134">displayName</span></span>|<span data-ttu-id="0e31a-135">字符串</span><span class="sxs-lookup"><span data-stu-id="0e31a-135">String</span></span>|<span data-ttu-id="0e31a-136">此显示名称的组。</span><span class="sxs-lookup"><span data-stu-id="0e31a-136">The display name for this policy.</span></span>|
|<span data-ttu-id="0e31a-137">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="0e31a-137">isAppliedToOrganization</span></span>|<span data-ttu-id="0e31a-138">布尔</span><span class="sxs-lookup"><span data-stu-id="0e31a-138">Boolean</span></span>|<span data-ttu-id="0e31a-139">指示是否应当将此功能推出策略应用于整个组织。</span><span class="sxs-lookup"><span data-stu-id="0e31a-139">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="0e31a-140">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0e31a-140">isEnabled</span></span>|<span data-ttu-id="0e31a-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e31a-141">Boolean</span></span>|<span data-ttu-id="0e31a-142">指示是否启用功能推出。</span><span class="sxs-lookup"><span data-stu-id="0e31a-142">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="0e31a-143">响应</span><span class="sxs-lookup"><span data-stu-id="0e31a-143">Response</span></span>

<span data-ttu-id="0e31a-144">如果成功，此方法返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0e31a-144">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0e31a-145">示例</span><span class="sxs-lookup"><span data-stu-id="0e31a-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e31a-146">请求</span><span class="sxs-lookup"><span data-stu-id="0e31a-146">Request</span></span>

<span data-ttu-id="0e31a-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0e31a-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e31a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e31a-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_featurerolloutpolicy_policies"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/featureRolloutPolicies/d7ab4886-d7f0-441b-a5e6-e62d7328d18a
Content-type: application/json

{
  "displayName": "PasswordHashSync Rollout Policy",
  "description": "PasswordHashSync Rollout Policy",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```
# <a name="c"></a>[<span data-ttu-id="0e31a-149">C#</span><span class="sxs-lookup"><span data-stu-id="0e31a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-featurerolloutpolicy-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e31a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e31a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-featurerolloutpolicy-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e31a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e31a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-featurerolloutpolicy-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e31a-152">Java</span><span class="sxs-lookup"><span data-stu-id="0e31a-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-featurerolloutpolicy-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0e31a-153">响应</span><span class="sxs-lookup"><span data-stu-id="0e31a-153">Response</span></span>

<span data-ttu-id="0e31a-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0e31a-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update featurerolloutpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


