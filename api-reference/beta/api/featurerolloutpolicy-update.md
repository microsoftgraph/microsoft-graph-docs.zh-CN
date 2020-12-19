---
title: 更新 featureRolloutPolicy
description: 更新 featurerolloutpolicy 对象的属性。
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 676983e4fbffcbe9edf3feae83c8344c52cf4596
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719942"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="2f9e6-103">更新 featurerolloutpolicy</span><span class="sxs-lookup"><span data-stu-id="2f9e6-103">Update featurerolloutpolicy</span></span>

<span data-ttu-id="2f9e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f9e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f9e6-105">更新 [featureRolloutPolicy 对象](../resources/featurerolloutpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-105">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f9e6-106">权限</span><span class="sxs-lookup"><span data-stu-id="2f9e6-106">Permissions</span></span>

<span data-ttu-id="2f9e6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f9e6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f9e6-109">Permission type</span></span>                        | <span data-ttu-id="2f9e6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f9e6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2f9e6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f9e6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f9e6-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="2f9e6-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="2f9e6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f9e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f9e6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-114">Not supported.</span></span> |
| <span data-ttu-id="2f9e6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f9e6-115">Application</span></span>                            | <span data-ttu-id="2f9e6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f9e6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f9e6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2f9e6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f9e6-118">Request headers</span></span>

| <span data-ttu-id="2f9e6-119">名称</span><span class="sxs-lookup"><span data-stu-id="2f9e6-119">Name</span></span>       | <span data-ttu-id="2f9e6-120">说明</span><span class="sxs-lookup"><span data-stu-id="2f9e6-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2f9e6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f9e6-121">Authorization</span></span> | <span data-ttu-id="2f9e6-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2f9e6-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f9e6-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f9e6-123">Request body</span></span>

<span data-ttu-id="2f9e6-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2f9e6-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2f9e6-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2f9e6-127">属性</span><span class="sxs-lookup"><span data-stu-id="2f9e6-127">Property</span></span>     | <span data-ttu-id="2f9e6-128">类型</span><span class="sxs-lookup"><span data-stu-id="2f9e6-128">Type</span></span>        | <span data-ttu-id="2f9e6-129">说明</span><span class="sxs-lookup"><span data-stu-id="2f9e6-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2f9e6-130">说明</span><span class="sxs-lookup"><span data-stu-id="2f9e6-130">description</span></span>|<span data-ttu-id="2f9e6-131">String</span><span class="sxs-lookup"><span data-stu-id="2f9e6-131">String</span></span>|<span data-ttu-id="2f9e6-132">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-132">A description for this policy.</span></span>|
|<span data-ttu-id="2f9e6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2f9e6-133">displayName</span></span>|<span data-ttu-id="2f9e6-134">String</span><span class="sxs-lookup"><span data-stu-id="2f9e6-134">String</span></span>|<span data-ttu-id="2f9e6-135">此显示名称的策略。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-135">The display name for this policy.</span></span>|
|<span data-ttu-id="2f9e6-136">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="2f9e6-136">isAppliedToOrganization</span></span>|<span data-ttu-id="2f9e6-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f9e6-137">Boolean</span></span>|<span data-ttu-id="2f9e6-138">指示此功能推出策略是否应该应用于整个组织。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-138">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="2f9e6-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="2f9e6-139">isEnabled</span></span>|<span data-ttu-id="2f9e6-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f9e6-140">Boolean</span></span>|<span data-ttu-id="2f9e6-141">指示是否启用功能推出。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-141">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="2f9e6-142">响应</span><span class="sxs-lookup"><span data-stu-id="2f9e6-142">Response</span></span>

<span data-ttu-id="2f9e6-143">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-143">If successful, this method returns a `200 OK` response code and an updated [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f9e6-144">示例</span><span class="sxs-lookup"><span data-stu-id="2f9e6-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f9e6-145">请求</span><span class="sxs-lookup"><span data-stu-id="2f9e6-145">Request</span></span>

<span data-ttu-id="2f9e6-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_featurerolloutpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/d7ab4886-d7f0-441b-a5e6-e62d7328d18a
Content-type: application/json

{
  "displayName": "PasswordHashSync Rollout Policy",
  "description": "PasswordHashSync Rollout Policy",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="response"></a><span data-ttu-id="2f9e6-147">响应</span><span class="sxs-lookup"><span data-stu-id="2f9e6-147">Response</span></span>

<span data-ttu-id="2f9e6-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-148">The following is an example of the response.</span></span>

> <span data-ttu-id="2f9e6-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2f9e6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
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


