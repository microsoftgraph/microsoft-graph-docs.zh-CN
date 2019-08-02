---
title: 创建 featureRolloutPolicy
description: 创建新的 featureRolloutPolicy 对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 716fa19e8fcccc69a33e53a22360638545ec81f5
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062105"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="f8858-103">创建 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="f8858-103">Create featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8858-104">创建新的[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f8858-104">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8858-105">权限</span><span class="sxs-lookup"><span data-stu-id="f8858-105">Permissions</span></span>

<span data-ttu-id="f8858-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8858-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8858-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8858-108">Permission type</span></span>                        | <span data-ttu-id="f8858-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8858-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f8858-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8858-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8858-111">FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="f8858-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="f8858-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8858-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8858-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8858-113">Not supported.</span></span> |
| <span data-ttu-id="f8858-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8858-114">Application</span></span>                            | <span data-ttu-id="f8858-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8858-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8858-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8858-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f8858-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8858-117">Request headers</span></span>

| <span data-ttu-id="f8858-118">名称</span><span class="sxs-lookup"><span data-stu-id="f8858-118">Name</span></span>          | <span data-ttu-id="f8858-119">说明</span><span class="sxs-lookup"><span data-stu-id="f8858-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f8858-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8858-120">Authorization</span></span> | <span data-ttu-id="f8858-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f8858-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8858-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8858-122">Request body</span></span>

<span data-ttu-id="f8858-123">在请求正文中, 提供[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8858-123">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="f8858-124">下表显示创建[featureRolloutPolicy](../resources/featurerolloutpolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f8858-124">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="f8858-125">参数</span><span class="sxs-lookup"><span data-stu-id="f8858-125">Parameter</span></span> | <span data-ttu-id="f8858-126">类型</span><span class="sxs-lookup"><span data-stu-id="f8858-126">Type</span></span> | <span data-ttu-id="f8858-127">说明</span><span class="sxs-lookup"><span data-stu-id="f8858-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8858-128">displayName</span><span class="sxs-lookup"><span data-stu-id="f8858-128">displayName</span></span> |<span data-ttu-id="f8858-129">string</span><span class="sxs-lookup"><span data-stu-id="f8858-129">string</span></span> |<span data-ttu-id="f8858-130">此功能展示策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f8858-130">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="f8858-131">功能</span><span class="sxs-lookup"><span data-stu-id="f8858-131">feature</span></span> |<span data-ttu-id="f8858-132">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="f8858-132">stagedFeatureName</span></span> |<span data-ttu-id="f8858-133">将使用此策略进行推出的功能。</span><span class="sxs-lookup"><span data-stu-id="f8858-133">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="f8858-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f8858-134">isEnabled</span></span> |<span data-ttu-id="f8858-135">string</span><span class="sxs-lookup"><span data-stu-id="f8858-135">string</span></span> |<span data-ttu-id="f8858-136">指示是否启用功能展示。</span><span class="sxs-lookup"><span data-stu-id="f8858-136">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="f8858-137">响应</span><span class="sxs-lookup"><span data-stu-id="f8858-137">Response</span></span>

<span data-ttu-id="f8858-138">如果成功, 此方法在响应`201 Created`正文中返回响应代码和新的[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f8858-138">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f8858-139">示例</span><span class="sxs-lookup"><span data-stu-id="f8858-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8858-140">请求</span><span class="sxs-lookup"><span data-stu-id="f8858-140">Request</span></span>

<span data-ttu-id="f8858-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f8858-141">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f8858-142">响应</span><span class="sxs-lookup"><span data-stu-id="f8858-142">Response</span></span>

<span data-ttu-id="f8858-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f8858-143">The following is an example of the response.</span></span>

> <span data-ttu-id="f8858-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f8858-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
