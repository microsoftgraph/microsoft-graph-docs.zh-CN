---
title: 获取 featureRolloutPolicy
description: 检索 featurerolloutpolicy 对象的属性和关系。
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5cd9830833ed06febf4b1b66b77d3ca4f72c52f8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436125"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="7ba90-103">获取 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="7ba90-103">Get featureRolloutPolicy</span></span>

<span data-ttu-id="7ba90-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ba90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ba90-105">检索 [featureRolloutPolicy 对象的属性和](../resources/featurerolloutpolicy.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="7ba90-105">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ba90-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7ba90-106">Permissions</span></span>

<span data-ttu-id="7ba90-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ba90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7ba90-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ba90-109">Permission type</span></span>                        | <span data-ttu-id="7ba90-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7ba90-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7ba90-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ba90-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ba90-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="7ba90-112">Policy.Read.All</span></span> |
| <span data-ttu-id="7ba90-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ba90-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ba90-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ba90-114">Not supported.</span></span> |
| <span data-ttu-id="7ba90-115">Application</span><span class="sxs-lookup"><span data-stu-id="7ba90-115">Application</span></span>                            | <span data-ttu-id="7ba90-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ba90-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ba90-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ba90-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7ba90-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7ba90-118">Optional query parameters</span></span>

<span data-ttu-id="7ba90-119">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7ba90-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="7ba90-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7ba90-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ba90-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ba90-121">Request headers</span></span>

| <span data-ttu-id="7ba90-122">名称</span><span class="sxs-lookup"><span data-stu-id="7ba90-122">Name</span></span>      |<span data-ttu-id="7ba90-123">说明</span><span class="sxs-lookup"><span data-stu-id="7ba90-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7ba90-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ba90-124">Authorization</span></span> | <span data-ttu-id="7ba90-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7ba90-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ba90-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ba90-126">Request body</span></span>

<span data-ttu-id="7ba90-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7ba90-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ba90-128">响应</span><span class="sxs-lookup"><span data-stu-id="7ba90-128">Response</span></span>

<span data-ttu-id="7ba90-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` 请求 [的 featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7ba90-129">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7ba90-130">示例</span><span class="sxs-lookup"><span data-stu-id="7ba90-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7ba90-131">请求</span><span class="sxs-lookup"><span data-stu-id="7ba90-131">Request</span></span>

<span data-ttu-id="7ba90-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7ba90-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ba90-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ba90-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="c"></a>[<span data-ttu-id="7ba90-134">C#</span><span class="sxs-lookup"><span data-stu-id="7ba90-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ba90-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ba90-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ba90-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ba90-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ba90-137">Java</span><span class="sxs-lookup"><span data-stu-id="7ba90-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7ba90-138">响应</span><span class="sxs-lookup"><span data-stu-id="7ba90-138">Response</span></span>

<span data-ttu-id="7ba90-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7ba90-139">The following is an example of the response.</span></span>

> <span data-ttu-id="7ba90-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7ba90-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="request"></a><span data-ttu-id="7ba90-142">请求</span><span class="sxs-lookup"><span data-stu-id="7ba90-142">Request</span></span>

<span data-ttu-id="7ba90-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7ba90-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ba90-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ba90-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="c"></a>[<span data-ttu-id="7ba90-145">C#</span><span class="sxs-lookup"><span data-stu-id="7ba90-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ba90-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ba90-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ba90-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ba90-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ba90-148">Java</span><span class="sxs-lookup"><span data-stu-id="7ba90-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7ba90-149">响应</span><span class="sxs-lookup"><span data-stu-id="7ba90-149">Response</span></span>

<span data-ttu-id="7ba90-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7ba90-150">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="7ba90-151">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7ba90-151">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7ba90-152">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7ba90-152">All the properties will be returned from an actual call.</span></span>

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


