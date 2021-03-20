---
title: 获取 featureRolloutPolicy
description: 检索 featurerolloutpolicy 对象的属性和关系。
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 956f5cada595471a1e9425b1399c69b4f4bc728c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955922"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="62a9c-103">获取 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="62a9c-103">Get featureRolloutPolicy</span></span>

<span data-ttu-id="62a9c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62a9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62a9c-105">检索 [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="62a9c-105">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="62a9c-106">权限</span><span class="sxs-lookup"><span data-stu-id="62a9c-106">Permissions</span></span>

<span data-ttu-id="62a9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62a9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62a9c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="62a9c-109">Permission type</span></span>                        | <span data-ttu-id="62a9c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62a9c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="62a9c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62a9c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="62a9c-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62a9c-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="62a9c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62a9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62a9c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="62a9c-114">Not supported.</span></span> |
| <span data-ttu-id="62a9c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="62a9c-115">Application</span></span>                            | <span data-ttu-id="62a9c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="62a9c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="62a9c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62a9c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62a9c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="62a9c-118">Optional query parameters</span></span>

<span data-ttu-id="62a9c-119">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="62a9c-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="62a9c-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="62a9c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="62a9c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="62a9c-121">Request headers</span></span>

| <span data-ttu-id="62a9c-122">名称</span><span class="sxs-lookup"><span data-stu-id="62a9c-122">Name</span></span>      |<span data-ttu-id="62a9c-123">说明</span><span class="sxs-lookup"><span data-stu-id="62a9c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="62a9c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="62a9c-124">Authorization</span></span> | <span data-ttu-id="62a9c-125">Bearer {token}。</span><span class="sxs-lookup"><span data-stu-id="62a9c-125">Bearer {token}.</span></span> <span data-ttu-id="62a9c-126">必需</span><span class="sxs-lookup"><span data-stu-id="62a9c-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="62a9c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="62a9c-127">Request body</span></span>

<span data-ttu-id="62a9c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="62a9c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62a9c-129">响应</span><span class="sxs-lookup"><span data-stu-id="62a9c-129">Response</span></span>

<span data-ttu-id="62a9c-130">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="62a9c-130">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62a9c-131">示例</span><span class="sxs-lookup"><span data-stu-id="62a9c-131">Examples</span></span>

### <a name="example-1-get-a-feature-rollout-policy"></a><span data-ttu-id="62a9c-132">示例 1：获取功能推出策略</span><span class="sxs-lookup"><span data-stu-id="62a9c-132">Example 1: Get a feature rollout policy</span></span>

#### <a name="request"></a><span data-ttu-id="62a9c-133">请求</span><span class="sxs-lookup"><span data-stu-id="62a9c-133">Request</span></span>

<span data-ttu-id="62a9c-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="62a9c-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
#### <a name="response"></a><span data-ttu-id="62a9c-135">响应</span><span class="sxs-lookup"><span data-stu-id="62a9c-135">Response</span></span>

<span data-ttu-id="62a9c-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="62a9c-136">The following is an example of the response.</span></span>

> <span data-ttu-id="62a9c-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="62a9c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="example-2-get-a-feature-rollout-policy-and-expand-appliesto"></a><span data-ttu-id="62a9c-139">示例 2：获取功能推出策略并展开 appliesTo</span><span class="sxs-lookup"><span data-stu-id="62a9c-139">Example 2: Get a feature rollout policy and expand appliesTo</span></span>

#### <a name="request"></a><span data-ttu-id="62a9c-140">请求</span><span class="sxs-lookup"><span data-stu-id="62a9c-140">Request</span></span>

<span data-ttu-id="62a9c-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="62a9c-141">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy_expandAppliesTo_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```

#### <a name="response"></a><span data-ttu-id="62a9c-142">响应</span><span class="sxs-lookup"><span data-stu-id="62a9c-142">Response</span></span>

<span data-ttu-id="62a9c-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="62a9c-143">The following is an example of the response.</span></span>

> <span data-ttu-id="62a9c-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="62a9c-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false,
  "appliesTo": [
    {
      "id": "2441b489-4f12-4882-b039-8f6006bd66da",
      "objectType": "group"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


