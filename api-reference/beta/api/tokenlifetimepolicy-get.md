---
title: 获取 tokenLifetimePolicy
description: 检索 tokenLifetimePolicy 对象的属性和关系。
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 14536ede77b27ab888d3c4d845ddb75f0579e3ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062253"
---
# <a name="get-tokenlifetimepolicy"></a><span data-ttu-id="7f67e-103">获取 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="7f67e-103">Get tokenLifetimePolicy</span></span>

<span data-ttu-id="7f67e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f67e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f67e-105">检索 [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7f67e-105">Retrieve the properties and relationships of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f67e-106">权限</span><span class="sxs-lookup"><span data-stu-id="7f67e-106">Permissions</span></span>

<span data-ttu-id="7f67e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f67e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f67e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f67e-109">Permission type</span></span>                        | <span data-ttu-id="7f67e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f67e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7f67e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f67e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f67e-112">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f67e-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="7f67e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f67e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f67e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f67e-114">Not supported.</span></span> |
| <span data-ttu-id="7f67e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f67e-115">Application</span></span>                            | <span data-ttu-id="7f67e-116">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f67e-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f67e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f67e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f67e-118">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="7f67e-118">Optional query parameters</span></span>

<span data-ttu-id="7f67e-119">此方法支持 `$expand` 和 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7f67e-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="7f67e-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7f67e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="7f67e-121">使用时 `$expand` ，请确保您的应用程序请求读取扩展的对象的权限。</span><span class="sxs-lookup"><span data-stu-id="7f67e-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f67e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f67e-122">Request headers</span></span>

| <span data-ttu-id="7f67e-123">名称</span><span class="sxs-lookup"><span data-stu-id="7f67e-123">Name</span></span>      |<span data-ttu-id="7f67e-124">说明</span><span class="sxs-lookup"><span data-stu-id="7f67e-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7f67e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f67e-125">Authorization</span></span> | <span data-ttu-id="7f67e-126">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="7f67e-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f67e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f67e-127">Request body</span></span>

<span data-ttu-id="7f67e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f67e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f67e-129">响应</span><span class="sxs-lookup"><span data-stu-id="7f67e-129">Response</span></span>

<span data-ttu-id="7f67e-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f67e-130">If successful, this method returns a `200 OK` response code and the requested [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7f67e-131">示例</span><span class="sxs-lookup"><span data-stu-id="7f67e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7f67e-132">请求</span><span class="sxs-lookup"><span data-stu-id="7f67e-132">Request</span></span>

<span data-ttu-id="7f67e-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7f67e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f67e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f67e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="7f67e-135">C#</span><span class="sxs-lookup"><span data-stu-id="7f67e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenlifetimepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f67e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f67e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenlifetimepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f67e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f67e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenlifetimepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7f67e-138">响应</span><span class="sxs-lookup"><span data-stu-id="7f67e-138">Response</span></span>

<span data-ttu-id="7f67e-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7f67e-139">The following is an example of the response.</span></span>

> <span data-ttu-id="7f67e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7f67e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Get tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


