---
title: 列出 featureRolloutPolicies
description: 检索 featureRolloutPolicy 对象的列表。
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b594b19d420ec794001851132457824691794c9c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436986"
---
# <a name="list-featurerolloutpolicies"></a><span data-ttu-id="8bc38-103">列出 featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="8bc38-103">List featureRolloutPolicies</span></span>

<span data-ttu-id="8bc38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bc38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bc38-105">检索 [featureRolloutPolicy 对象](../resources/featurerolloutpolicy.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="8bc38-105">Retrieve a list of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bc38-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8bc38-106">Permissions</span></span>

<span data-ttu-id="8bc38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8bc38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8bc38-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8bc38-109">Permission type</span></span>                        | <span data-ttu-id="8bc38-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8bc38-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8bc38-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8bc38-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8bc38-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bc38-112">Policy.Read.All</span></span> |
| <span data-ttu-id="8bc38-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8bc38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bc38-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8bc38-114">Not supported.</span></span> |
| <span data-ttu-id="8bc38-115">Application</span><span class="sxs-lookup"><span data-stu-id="8bc38-115">Application</span></span>                            | <span data-ttu-id="8bc38-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8bc38-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bc38-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8bc38-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8bc38-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8bc38-118">Optional query parameters</span></span>

<span data-ttu-id="8bc38-119">此方法支持以下 OData 查询参数来帮助自定义响应： ， `$count` `$expand` ， `$filter` ， ， `$orderby` ， `$select` `$skip` `$top` 。</span><span class="sxs-lookup"><span data-stu-id="8bc38-119">This method supports the following OData query parameters to help customize the response: `$count`, `$expand`, `$filter`, `$orderby`, `$select`, `$skip`, `$top`.</span></span> <span data-ttu-id="8bc38-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="8bc38-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8bc38-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8bc38-121">Request headers</span></span>

| <span data-ttu-id="8bc38-122">名称</span><span class="sxs-lookup"><span data-stu-id="8bc38-122">Name</span></span>      |<span data-ttu-id="8bc38-123">说明</span><span class="sxs-lookup"><span data-stu-id="8bc38-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8bc38-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bc38-124">Authorization</span></span> | <span data-ttu-id="8bc38-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8bc38-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bc38-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8bc38-126">Request body</span></span>

<span data-ttu-id="8bc38-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8bc38-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bc38-128">响应</span><span class="sxs-lookup"><span data-stu-id="8bc38-128">Response</span></span>

<span data-ttu-id="8bc38-129">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8bc38-129">If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8bc38-130">示例</span><span class="sxs-lookup"><span data-stu-id="8bc38-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8bc38-131">请求</span><span class="sxs-lookup"><span data-stu-id="8bc38-131">Request</span></span>

<span data-ttu-id="8bc38-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8bc38-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8bc38-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bc38-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies
```
# <a name="c"></a>[<span data-ttu-id="8bc38-134">C#</span><span class="sxs-lookup"><span data-stu-id="8bc38-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bc38-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bc38-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bc38-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bc38-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8bc38-137">Java</span><span class="sxs-lookup"><span data-stu-id="8bc38-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8bc38-138">响应</span><span class="sxs-lookup"><span data-stu-id="8bc38-138">Response</span></span>

<span data-ttu-id="8bc38-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8bc38-139">The following is an example of the response.</span></span>

> <span data-ttu-id="8bc38-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8bc38-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "e3c2f23a-edd2-43a8-849f-154e70794ac5",
      "displayName": "PassthroughAuthentication rollout policy",
      "description": "PassthroughAuthentication rollout policy",
      "feature": "passthroughAuthentication",
      "isEnabled": true,
      "isAppliedToOrganization": false
    },
    {
      "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
      "displayName": "SeamlessSso rollout policy",
      "description": "SeamlessSso rollout policy",
      "feature": "seamlessSso",
      "isEnabled": true,
      "isAppliedToOrganization": false
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List featureRolloutPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


