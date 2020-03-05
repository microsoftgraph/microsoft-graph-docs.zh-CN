---
title: 获取 featureRolloutPolicy
description: 检索 featurerolloutpolicy 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 155d9398a981c8d3a478f92ac61de04d97f873a0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421758"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="14fb0-103">获取 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="14fb0-103">Get featureRolloutPolicy</span></span>

<span data-ttu-id="14fb0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="14fb0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14fb0-105">检索[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14fb0-105">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="14fb0-106">权限</span><span class="sxs-lookup"><span data-stu-id="14fb0-106">Permissions</span></span>

<span data-ttu-id="14fb0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14fb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14fb0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="14fb0-109">Permission type</span></span>                        | <span data-ttu-id="14fb0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14fb0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="14fb0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14fb0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="14fb0-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="14fb0-112">Policy.Read.All</span></span> |
| <span data-ttu-id="14fb0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14fb0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14fb0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="14fb0-114">Not supported.</span></span> |
| <span data-ttu-id="14fb0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="14fb0-115">Application</span></span>                            | <span data-ttu-id="14fb0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="14fb0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14fb0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14fb0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14fb0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="14fb0-118">Optional query parameters</span></span>

<span data-ttu-id="14fb0-119">此方法支持`$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="14fb0-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="14fb0-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="14fb0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="14fb0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="14fb0-121">Request headers</span></span>

| <span data-ttu-id="14fb0-122">名称</span><span class="sxs-lookup"><span data-stu-id="14fb0-122">Name</span></span>      |<span data-ttu-id="14fb0-123">说明</span><span class="sxs-lookup"><span data-stu-id="14fb0-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="14fb0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="14fb0-124">Authorization</span></span> | <span data-ttu-id="14fb0-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="14fb0-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="14fb0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="14fb0-126">Request body</span></span>

<span data-ttu-id="14fb0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="14fb0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14fb0-128">响应</span><span class="sxs-lookup"><span data-stu-id="14fb0-128">Response</span></span>

<span data-ttu-id="14fb0-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[featureRolloutPolicy](../resources/featurerolloutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="14fb0-129">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14fb0-130">示例</span><span class="sxs-lookup"><span data-stu-id="14fb0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14fb0-131">请求</span><span class="sxs-lookup"><span data-stu-id="14fb0-131">Request</span></span>

<span data-ttu-id="14fb0-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="14fb0-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14fb0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="14fb0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="c"></a>[<span data-ttu-id="14fb0-134">C#</span><span class="sxs-lookup"><span data-stu-id="14fb0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14fb0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14fb0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14fb0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14fb0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14fb0-137">响应</span><span class="sxs-lookup"><span data-stu-id="14fb0-137">Response</span></span>

<span data-ttu-id="14fb0-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="14fb0-138">The following is an example of the response.</span></span>

> <span data-ttu-id="14fb0-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="14fb0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="request"></a><span data-ttu-id="14fb0-141">请求</span><span class="sxs-lookup"><span data-stu-id="14fb0-141">Request</span></span>

<span data-ttu-id="14fb0-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="14fb0-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14fb0-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="14fb0-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="c"></a>[<span data-ttu-id="14fb0-144">C#</span><span class="sxs-lookup"><span data-stu-id="14fb0-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14fb0-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14fb0-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14fb0-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14fb0-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14fb0-147">响应</span><span class="sxs-lookup"><span data-stu-id="14fb0-147">Response</span></span>

<span data-ttu-id="14fb0-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="14fb0-148">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="14fb0-149">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="14fb0-149">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="14fb0-150">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="14fb0-150">All the properties will be returned from an actual call.</span></span>

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
