---
title: 获取 claimsMappingPolicy
description: 检索 claimsMappingPolicy 对象的属性和关系。
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 16e86b3e8be0ff7ecc3db9c0eeab763ae78a350f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50432898"
---
# <a name="get-claimsmappingpolicy"></a><span data-ttu-id="0fe22-103">获取 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="0fe22-103">Get claimsMappingPolicy</span></span>

<span data-ttu-id="0fe22-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fe22-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0fe22-105">检索 [claimsMappingPolicy 对象的属性和](../resources/claimsmappingpolicy.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="0fe22-105">Retrieve the properties and relationships of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fe22-106">权限</span><span class="sxs-lookup"><span data-stu-id="0fe22-106">Permissions</span></span>

<span data-ttu-id="0fe22-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0fe22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0fe22-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0fe22-109">Permission type</span></span>                        | <span data-ttu-id="0fe22-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0fe22-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0fe22-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0fe22-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0fe22-112">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fe22-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="0fe22-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0fe22-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fe22-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0fe22-114">Not supported.</span></span> |
| <span data-ttu-id="0fe22-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0fe22-115">Application</span></span>                            | <span data-ttu-id="0fe22-116">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fe22-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fe22-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0fe22-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0fe22-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0fe22-118">Optional query parameters</span></span>

<span data-ttu-id="0fe22-119">此方法支持和 `$expand` `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0fe22-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="0fe22-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0fe22-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="0fe22-121">使用 `$expand` 时，请确保你的应用请求读取扩展对象的权限。</span><span class="sxs-lookup"><span data-stu-id="0fe22-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fe22-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0fe22-122">Request headers</span></span>

| <span data-ttu-id="0fe22-123">名称</span><span class="sxs-lookup"><span data-stu-id="0fe22-123">Name</span></span>      |<span data-ttu-id="0fe22-124">说明</span><span class="sxs-lookup"><span data-stu-id="0fe22-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0fe22-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fe22-125">Authorization</span></span> | <span data-ttu-id="0fe22-126">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0fe22-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fe22-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0fe22-127">Request body</span></span>

<span data-ttu-id="0fe22-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0fe22-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fe22-129">响应</span><span class="sxs-lookup"><span data-stu-id="0fe22-129">Response</span></span>

<span data-ttu-id="0fe22-130">如果成功，此方法在响应正文中返回响应代码和请求 `200 OK` [的 claimsMappingPolicy](../resources/claimsmappingpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0fe22-130">If successful, this method returns a `200 OK` response code and the requested [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0fe22-131">示例</span><span class="sxs-lookup"><span data-stu-id="0fe22-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0fe22-132">请求</span><span class="sxs-lookup"><span data-stu-id="0fe22-132">Request</span></span>

<span data-ttu-id="0fe22-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0fe22-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0fe22-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fe22-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="0fe22-135">C#</span><span class="sxs-lookup"><span data-stu-id="0fe22-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fe22-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fe22-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fe22-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fe22-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fe22-138">Java</span><span class="sxs-lookup"><span data-stu-id="0fe22-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-claimsmappingpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0fe22-139">响应</span><span class="sxs-lookup"><span data-stu-id="0fe22-139">Response</span></span>

<span data-ttu-id="0fe22-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0fe22-140">The following is an example of the response.</span></span>

> <span data-ttu-id="0fe22-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0fe22-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
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
  "description": "Get claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

