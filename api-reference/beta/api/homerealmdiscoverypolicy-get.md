---
title: 获取 homeRealmDiscoveryPolicy
description: 检索 homeRealmDiscoveryPolicy 对象的属性和关系。
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8c40537df3bd16056b4d95b3788cffd18ee03da2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435712"
---
# <a name="get-homerealmdiscoverypolicy"></a><span data-ttu-id="72b75-103">获取 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="72b75-103">Get homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="72b75-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72b75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72b75-105">检索 [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="72b75-105">Retrieve the properties and relationships of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="72b75-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="72b75-106">Permissions</span></span>

<span data-ttu-id="72b75-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72b75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72b75-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="72b75-109">Permission type</span></span>                        | <span data-ttu-id="72b75-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72b75-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="72b75-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72b75-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="72b75-112">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="72b75-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="72b75-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72b75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72b75-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="72b75-114">Not supported.</span></span> |
| <span data-ttu-id="72b75-115">Application</span><span class="sxs-lookup"><span data-stu-id="72b75-115">Application</span></span>                            | <span data-ttu-id="72b75-116">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="72b75-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="72b75-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72b75-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72b75-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="72b75-118">Optional query parameters</span></span>

<span data-ttu-id="72b75-119">此方法支持和 `$expand` `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="72b75-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="72b75-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="72b75-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="72b75-121">使用 `$expand` 时，请确保你的应用请求读取扩展对象的权限。</span><span class="sxs-lookup"><span data-stu-id="72b75-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72b75-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="72b75-122">Request headers</span></span>

| <span data-ttu-id="72b75-123">名称</span><span class="sxs-lookup"><span data-stu-id="72b75-123">Name</span></span>      |<span data-ttu-id="72b75-124">说明</span><span class="sxs-lookup"><span data-stu-id="72b75-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72b75-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="72b75-125">Authorization</span></span> | <span data-ttu-id="72b75-126">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="72b75-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="72b75-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="72b75-127">Request body</span></span>

<span data-ttu-id="72b75-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="72b75-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72b75-129">响应</span><span class="sxs-lookup"><span data-stu-id="72b75-129">Response</span></span>

<span data-ttu-id="72b75-130">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72b75-130">If successful, this method returns a `200 OK` response code and the requested [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72b75-131">示例</span><span class="sxs-lookup"><span data-stu-id="72b75-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72b75-132">请求</span><span class="sxs-lookup"><span data-stu-id="72b75-132">Request</span></span>

<span data-ttu-id="72b75-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="72b75-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72b75-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="72b75-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="72b75-135">C#</span><span class="sxs-lookup"><span data-stu-id="72b75-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72b75-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72b75-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72b75-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72b75-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72b75-138">Java</span><span class="sxs-lookup"><span data-stu-id="72b75-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="72b75-139">响应</span><span class="sxs-lookup"><span data-stu-id="72b75-139">Response</span></span>

<span data-ttu-id="72b75-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="72b75-140">The following is an example of the response.</span></span>

> <span data-ttu-id="72b75-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="72b75-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


