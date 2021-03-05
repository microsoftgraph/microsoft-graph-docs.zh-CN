---
title: 获取 tokenIssuancePolicy
description: 检索 tokenIssuancePolicy 对象的属性和关系。
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f4a7025ea69e9224d04efc81f86c038eb20a3465
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433759"
---
# <a name="get-tokenissuancepolicy"></a><span data-ttu-id="5e877-103">获取 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="5e877-103">Get tokenIssuancePolicy</span></span>

<span data-ttu-id="5e877-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e877-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e877-105">检索 [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5e877-105">Retrieve the properties and relationships of a [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e877-106">权限</span><span class="sxs-lookup"><span data-stu-id="5e877-106">Permissions</span></span>

<span data-ttu-id="5e877-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e877-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e877-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e877-109">Permission type</span></span>                        | <span data-ttu-id="5e877-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e877-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5e877-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e877-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5e877-112">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5e877-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="5e877-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e877-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e877-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e877-114">Not supported.</span></span> |
| <span data-ttu-id="5e877-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e877-115">Application</span></span>                            | <span data-ttu-id="5e877-116">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5e877-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e877-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e877-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenIssuancePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e877-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5e877-118">Optional query parameters</span></span>

<span data-ttu-id="5e877-119">此方法支持和 `$expand` `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5e877-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="5e877-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5e877-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="5e877-121">使用 `$expand` 时，请确保你的应用请求读取扩展对象的权限。</span><span class="sxs-lookup"><span data-stu-id="5e877-121">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e877-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e877-122">Request headers</span></span>

| <span data-ttu-id="5e877-123">名称</span><span class="sxs-lookup"><span data-stu-id="5e877-123">Name</span></span>      |<span data-ttu-id="5e877-124">说明</span><span class="sxs-lookup"><span data-stu-id="5e877-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5e877-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e877-125">Authorization</span></span> | <span data-ttu-id="5e877-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e877-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e877-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e877-128">Request body</span></span>

<span data-ttu-id="5e877-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5e877-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e877-130">响应</span><span class="sxs-lookup"><span data-stu-id="5e877-130">Response</span></span>

<span data-ttu-id="5e877-131">如果成功，此方法在响应正文中返回响应代码和请求 `200 OK` [的 tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5e877-131">If successful, this method returns a `200 OK` response code and the requested [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5e877-132">示例</span><span class="sxs-lookup"><span data-stu-id="5e877-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5e877-133">请求</span><span class="sxs-lookup"><span data-stu-id="5e877-133">Request</span></span>

<span data-ttu-id="5e877-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5e877-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e877-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e877-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenIssuancePolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="5e877-136">C#</span><span class="sxs-lookup"><span data-stu-id="5e877-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenissuancepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e877-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e877-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenissuancepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e877-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e877-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenissuancepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e877-139">Java</span><span class="sxs-lookup"><span data-stu-id="5e877-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tokenissuancepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="5e877-140">响应</span><span class="sxs-lookup"><span data-stu-id="5e877-140">Response</span></span>

<span data-ttu-id="5e877-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5e877-141">The following is an example of the response.</span></span>

> <span data-ttu-id="5e877-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5e877-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
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
  "description": "Get tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


