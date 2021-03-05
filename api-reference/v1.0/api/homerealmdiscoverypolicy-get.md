---
title: 获取 homeRealmDiscoveryPolicy
description: 检索 homeRealmDiscoveryPolicy 对象的属性和关系。
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 62cf25768b628dff2847a5d5d4859ac826fc259a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434333"
---
# <a name="get-homerealmdiscoverypolicy"></a><span data-ttu-id="783eb-103">获取 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="783eb-103">Get homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="783eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="783eb-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="783eb-105">检索 [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="783eb-105">Retrieve the properties and relationships of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="783eb-106">权限</span><span class="sxs-lookup"><span data-stu-id="783eb-106">Permissions</span></span>

<span data-ttu-id="783eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="783eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="783eb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="783eb-109">Permission type</span></span>                        | <span data-ttu-id="783eb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="783eb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="783eb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="783eb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="783eb-112">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="783eb-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="783eb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="783eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="783eb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="783eb-114">Not supported.</span></span> |
| <span data-ttu-id="783eb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="783eb-115">Application</span></span>                            | <span data-ttu-id="783eb-116">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="783eb-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="783eb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="783eb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="783eb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="783eb-118">Optional query parameters</span></span>

<span data-ttu-id="783eb-119">此方法支持和 `$expand` `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="783eb-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="783eb-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="783eb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="783eb-121">使用 `$expand` 时，请确保你的应用请求读取扩展对象的权限。</span><span class="sxs-lookup"><span data-stu-id="783eb-121">When using `$expand`, make sure that your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="783eb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="783eb-122">Request headers</span></span>

| <span data-ttu-id="783eb-123">名称</span><span class="sxs-lookup"><span data-stu-id="783eb-123">Name</span></span>      |<span data-ttu-id="783eb-124">说明</span><span class="sxs-lookup"><span data-stu-id="783eb-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="783eb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="783eb-125">Authorization</span></span> | <span data-ttu-id="783eb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="783eb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="783eb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="783eb-128">Request body</span></span>

<span data-ttu-id="783eb-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="783eb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="783eb-130">响应</span><span class="sxs-lookup"><span data-stu-id="783eb-130">Response</span></span>

<span data-ttu-id="783eb-131">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="783eb-131">If successful, this method returns a `200 OK` response code and the requested [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="783eb-132">示例</span><span class="sxs-lookup"><span data-stu-id="783eb-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="783eb-133">请求</span><span class="sxs-lookup"><span data-stu-id="783eb-133">Request</span></span>

<span data-ttu-id="783eb-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="783eb-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="783eb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="783eb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="783eb-136">C#</span><span class="sxs-lookup"><span data-stu-id="783eb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="783eb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="783eb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="783eb-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="783eb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="783eb-139">Java</span><span class="sxs-lookup"><span data-stu-id="783eb-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="783eb-140">响应</span><span class="sxs-lookup"><span data-stu-id="783eb-140">Response</span></span>

<span data-ttu-id="783eb-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="783eb-141">The following is an example of the response.</span></span>

> <span data-ttu-id="783eb-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="783eb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

