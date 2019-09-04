---
title: 获取 featureRolloutPolicy
description: 检索 featurerolloutpolicy 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7ddf2072116cdf7209c2bf24def5edda6aebadcf
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721717"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="f810e-103">获取 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="f810e-103">Get featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f810e-104">检索[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f810e-104">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f810e-105">权限</span><span class="sxs-lookup"><span data-stu-id="f810e-105">Permissions</span></span>

<span data-ttu-id="f810e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f810e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f810e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f810e-108">Permission type</span></span>                        | <span data-ttu-id="f810e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f810e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f810e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f810e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f810e-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="f810e-111">Policy.Read.All</span></span> |
| <span data-ttu-id="f810e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f810e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f810e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f810e-113">Not supported.</span></span> |
| <span data-ttu-id="f810e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f810e-114">Application</span></span>                            | <span data-ttu-id="f810e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f810e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f810e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f810e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f810e-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f810e-117">Optional query parameters</span></span>

<span data-ttu-id="f810e-118">此方法支持`$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f810e-118">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="f810e-119">有关一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f810e-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f810e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f810e-120">Request headers</span></span>

| <span data-ttu-id="f810e-121">名称</span><span class="sxs-lookup"><span data-stu-id="f810e-121">Name</span></span>      |<span data-ttu-id="f810e-122">说明</span><span class="sxs-lookup"><span data-stu-id="f810e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f810e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f810e-123">Authorization</span></span> | <span data-ttu-id="f810e-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f810e-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f810e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f810e-125">Request body</span></span>

<span data-ttu-id="f810e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f810e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f810e-127">响应</span><span class="sxs-lookup"><span data-stu-id="f810e-127">Response</span></span>

<span data-ttu-id="f810e-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f810e-128">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f810e-129">示例</span><span class="sxs-lookup"><span data-stu-id="f810e-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f810e-130">请求</span><span class="sxs-lookup"><span data-stu-id="f810e-130">Request</span></span>

<span data-ttu-id="f810e-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f810e-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f810e-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f810e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f810e-133">C#</span><span class="sxs-lookup"><span data-stu-id="f810e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f810e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f810e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f810e-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="f810e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f810e-136">响应</span><span class="sxs-lookup"><span data-stu-id="f810e-136">Response</span></span>

<span data-ttu-id="f810e-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f810e-137">The following is an example of the response.</span></span>

> <span data-ttu-id="f810e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f810e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="request"></a><span data-ttu-id="f810e-140">请求</span><span class="sxs-lookup"><span data-stu-id="f810e-140">Request</span></span>

<span data-ttu-id="f810e-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f810e-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f810e-142">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f810e-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f810e-143">C#</span><span class="sxs-lookup"><span data-stu-id="f810e-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f810e-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f810e-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f810e-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="f810e-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f810e-146">响应</span><span class="sxs-lookup"><span data-stu-id="f810e-146">Response</span></span>

<span data-ttu-id="f810e-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f810e-147">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="f810e-148">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f810e-148">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f810e-149">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f810e-149">All the properties will be returned from an actual call.</span></span>

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
