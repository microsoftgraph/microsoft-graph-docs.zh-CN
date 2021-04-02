---
title: 获取 featureRolloutPolicy
description: 检索 featurerolloutpolicy 对象的属性和关系。
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6cb7f140e29e15643850352ea2107b77b9a96495
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508635"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="c9635-103">获取 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c9635-103">Get featureRolloutPolicy</span></span>

<span data-ttu-id="c9635-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9635-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9635-105">检索 [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9635-105">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9635-106">权限</span><span class="sxs-lookup"><span data-stu-id="c9635-106">Permissions</span></span>

<span data-ttu-id="c9635-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9635-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c9635-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9635-109">Permission type</span></span>                        | <span data-ttu-id="c9635-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c9635-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c9635-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9635-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9635-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9635-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="c9635-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9635-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9635-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9635-114">Not supported.</span></span> |
| <span data-ttu-id="c9635-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9635-115">Application</span></span>                            | <span data-ttu-id="c9635-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9635-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9635-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9635-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9635-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c9635-118">Optional query parameters</span></span>

<span data-ttu-id="c9635-119">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c9635-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="c9635-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c9635-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9635-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9635-121">Request headers</span></span>

| <span data-ttu-id="c9635-122">名称</span><span class="sxs-lookup"><span data-stu-id="c9635-122">Name</span></span>      |<span data-ttu-id="c9635-123">说明</span><span class="sxs-lookup"><span data-stu-id="c9635-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c9635-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9635-124">Authorization</span></span> | <span data-ttu-id="c9635-125">Bearer {token}。</span><span class="sxs-lookup"><span data-stu-id="c9635-125">Bearer {token}.</span></span> <span data-ttu-id="c9635-126">必需</span><span class="sxs-lookup"><span data-stu-id="c9635-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9635-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9635-127">Request body</span></span>

<span data-ttu-id="c9635-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c9635-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9635-129">响应</span><span class="sxs-lookup"><span data-stu-id="c9635-129">Response</span></span>

<span data-ttu-id="c9635-130">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c9635-130">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9635-131">示例</span><span class="sxs-lookup"><span data-stu-id="c9635-131">Examples</span></span>

### <a name="example-1-get-a-feature-rollout-policy"></a><span data-ttu-id="c9635-132">示例 1：获取功能推出策略</span><span class="sxs-lookup"><span data-stu-id="c9635-132">Example 1: Get a feature rollout policy</span></span>

#### <a name="request"></a><span data-ttu-id="c9635-133">请求</span><span class="sxs-lookup"><span data-stu-id="c9635-133">Request</span></span>

<span data-ttu-id="c9635-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c9635-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c9635-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9635-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="c"></a>[<span data-ttu-id="c9635-136">C#</span><span class="sxs-lookup"><span data-stu-id="c9635-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9635-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9635-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9635-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9635-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9635-139">Java</span><span class="sxs-lookup"><span data-stu-id="c9635-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c9635-140">响应</span><span class="sxs-lookup"><span data-stu-id="c9635-140">Response</span></span>

<span data-ttu-id="c9635-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c9635-141">The following is an example of the response.</span></span>

> <span data-ttu-id="c9635-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c9635-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-feature-rollout-policy-and-expand-appliesto"></a><span data-ttu-id="c9635-144">示例 2：获取功能推出策略并展开 appliesTo</span><span class="sxs-lookup"><span data-stu-id="c9635-144">Example 2: Get a feature rollout policy and expand appliesTo</span></span>

#### <a name="request"></a><span data-ttu-id="c9635-145">请求</span><span class="sxs-lookup"><span data-stu-id="c9635-145">Request</span></span>

<span data-ttu-id="c9635-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c9635-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c9635-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9635-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy_expandAppliesTo_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="c"></a>[<span data-ttu-id="c9635-148">C#</span><span class="sxs-lookup"><span data-stu-id="c9635-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-expandappliesto-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9635-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9635-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-expandappliesto-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9635-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9635-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-expandappliesto-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9635-151">Java</span><span class="sxs-lookup"><span data-stu-id="c9635-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-expandappliesto-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c9635-152">响应</span><span class="sxs-lookup"><span data-stu-id="c9635-152">Response</span></span>

<span data-ttu-id="c9635-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c9635-153">The following is an example of the response.</span></span>

> <span data-ttu-id="c9635-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c9635-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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


