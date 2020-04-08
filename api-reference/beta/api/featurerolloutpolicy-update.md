---
title: 更新 featureRolloutPolicy
description: 更新 featurerolloutpolicy 对象的属性。
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d1e454f08649b631a694194a585a623e9c819702
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181096"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="3345f-103">更新 featurerolloutpolicy</span><span class="sxs-lookup"><span data-stu-id="3345f-103">Update featurerolloutpolicy</span></span>

<span data-ttu-id="3345f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3345f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3345f-105">更新[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3345f-105">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3345f-106">权限</span><span class="sxs-lookup"><span data-stu-id="3345f-106">Permissions</span></span>

<span data-ttu-id="3345f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3345f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3345f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3345f-109">Permission type</span></span>                        | <span data-ttu-id="3345f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3345f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3345f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3345f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3345f-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="3345f-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="3345f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3345f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3345f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3345f-114">Not supported.</span></span> |
| <span data-ttu-id="3345f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3345f-115">Application</span></span>                            | <span data-ttu-id="3345f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3345f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3345f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3345f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3345f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3345f-118">Request headers</span></span>

| <span data-ttu-id="3345f-119">名称</span><span class="sxs-lookup"><span data-stu-id="3345f-119">Name</span></span>       | <span data-ttu-id="3345f-120">说明</span><span class="sxs-lookup"><span data-stu-id="3345f-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3345f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3345f-121">Authorization</span></span> | <span data-ttu-id="3345f-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3345f-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3345f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3345f-123">Request body</span></span>

<span data-ttu-id="3345f-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="3345f-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3345f-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="3345f-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3345f-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="3345f-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3345f-127">属性</span><span class="sxs-lookup"><span data-stu-id="3345f-127">Property</span></span>     | <span data-ttu-id="3345f-128">类型</span><span class="sxs-lookup"><span data-stu-id="3345f-128">Type</span></span>        | <span data-ttu-id="3345f-129">说明</span><span class="sxs-lookup"><span data-stu-id="3345f-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3345f-130">说明</span><span class="sxs-lookup"><span data-stu-id="3345f-130">description</span></span>|<span data-ttu-id="3345f-131">String</span><span class="sxs-lookup"><span data-stu-id="3345f-131">String</span></span>|<span data-ttu-id="3345f-132">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="3345f-132">A description for this policy.</span></span>|
|<span data-ttu-id="3345f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3345f-133">displayName</span></span>|<span data-ttu-id="3345f-134">String</span><span class="sxs-lookup"><span data-stu-id="3345f-134">String</span></span>|<span data-ttu-id="3345f-135">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3345f-135">The display name for this policy.</span></span>|
|<span data-ttu-id="3345f-136">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="3345f-136">isAppliedToOrganization</span></span>|<span data-ttu-id="3345f-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="3345f-137">Boolean</span></span>|<span data-ttu-id="3345f-138">指示是否应将此功能展示策略应用于整个组织。</span><span class="sxs-lookup"><span data-stu-id="3345f-138">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="3345f-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3345f-139">isEnabled</span></span>|<span data-ttu-id="3345f-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="3345f-140">Boolean</span></span>|<span data-ttu-id="3345f-141">指示是否启用功能展示。</span><span class="sxs-lookup"><span data-stu-id="3345f-141">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="3345f-142">响应</span><span class="sxs-lookup"><span data-stu-id="3345f-142">Response</span></span>

<span data-ttu-id="3345f-143">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3345f-143">If successful, this method returns a `200 OK` response code and an updated [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3345f-144">示例</span><span class="sxs-lookup"><span data-stu-id="3345f-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3345f-145">请求</span><span class="sxs-lookup"><span data-stu-id="3345f-145">Request</span></span>

<span data-ttu-id="3345f-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3345f-146">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3345f-147">响应</span><span class="sxs-lookup"><span data-stu-id="3345f-147">Response</span></span>

<span data-ttu-id="3345f-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3345f-148">The following is an example of the response.</span></span>

> <span data-ttu-id="3345f-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3345f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
