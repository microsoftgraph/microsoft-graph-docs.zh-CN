---
title: 获取 featureRolloutPolicy
description: 检索 featurerolloutpolicy 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8c36c8db23e0550ac1d68aea363ce7921d82a3a0
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062108"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="eb9c0-103">获取 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="eb9c0-103">Get featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb9c0-104">检索[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-104">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb9c0-105">权限</span><span class="sxs-lookup"><span data-stu-id="eb9c0-105">Permissions</span></span>

<span data-ttu-id="eb9c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb9c0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb9c0-108">Permission type</span></span>                        | <span data-ttu-id="eb9c0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb9c0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="eb9c0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb9c0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb9c0-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb9c0-111">Policy.Read.All</span></span> |
| <span data-ttu-id="eb9c0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb9c0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb9c0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-113">Not supported.</span></span> |
| <span data-ttu-id="eb9c0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb9c0-114">Application</span></span>                            | <span data-ttu-id="eb9c0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb9c0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb9c0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb9c0-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="eb9c0-117">Optional query parameters</span></span>

<span data-ttu-id="eb9c0-118">此方法支持`$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-118">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="eb9c0-119">有关一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb9c0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb9c0-120">Request headers</span></span>

| <span data-ttu-id="eb9c0-121">名称</span><span class="sxs-lookup"><span data-stu-id="eb9c0-121">Name</span></span>      |<span data-ttu-id="eb9c0-122">说明</span><span class="sxs-lookup"><span data-stu-id="eb9c0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb9c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb9c0-123">Authorization</span></span> | <span data-ttu-id="eb9c0-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="eb9c0-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb9c0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb9c0-125">Request body</span></span>

<span data-ttu-id="eb9c0-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb9c0-127">响应</span><span class="sxs-lookup"><span data-stu-id="eb9c0-127">Response</span></span>

<span data-ttu-id="eb9c0-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-128">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb9c0-129">示例</span><span class="sxs-lookup"><span data-stu-id="eb9c0-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb9c0-130">请求</span><span class="sxs-lookup"><span data-stu-id="eb9c0-130">Request</span></span>

<span data-ttu-id="eb9c0-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="eb9c0-132">响应</span><span class="sxs-lookup"><span data-stu-id="eb9c0-132">Response</span></span>

<span data-ttu-id="eb9c0-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-133">The following is an example of the response.</span></span>

> <span data-ttu-id="eb9c0-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="request"></a><span data-ttu-id="eb9c0-136">请求</span><span class="sxs-lookup"><span data-stu-id="eb9c0-136">Request</span></span>

<span data-ttu-id="eb9c0-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```

### <a name="response"></a><span data-ttu-id="eb9c0-138">响应</span><span class="sxs-lookup"><span data-stu-id="eb9c0-138">Response</span></span>

<span data-ttu-id="eb9c0-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="eb9c0-140">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="eb9c0-141">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="eb9c0-141">All the properties will be returned from an actual call.</span></span>

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
