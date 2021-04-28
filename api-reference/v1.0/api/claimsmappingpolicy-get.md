---
title: 获取 claimsMappingPolicy
description: 检索 claimsMappingPolicy 对象的属性和关系。
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 74ab898eaf2d8d2985df7ebb4ebdb4a76f8afa43
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050561"
---
# <a name="get-claimsmappingpolicy"></a><span data-ttu-id="77856-103">获取 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="77856-103">Get claimsMappingPolicy</span></span>

<span data-ttu-id="77856-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77856-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="77856-105">检索 [claimsMappingPolicy](../resources/claimsmappingpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77856-105">Retrieve the properties and relationships of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="77856-106">权限</span><span class="sxs-lookup"><span data-stu-id="77856-106">Permissions</span></span>

<span data-ttu-id="77856-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77856-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77856-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="77856-109">Permission type</span></span>                        | <span data-ttu-id="77856-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77856-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="77856-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77856-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="77856-112">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="77856-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="77856-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77856-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77856-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="77856-114">Not supported.</span></span> |
| <span data-ttu-id="77856-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="77856-115">Application</span></span>                            | <span data-ttu-id="77856-116">Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="77856-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="77856-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77856-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77856-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="77856-118">Optional query parameters</span></span>

<span data-ttu-id="77856-119">此方法支持 `$expand` 和 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="77856-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="77856-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="77856-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="77856-121">使用 `$expand` 时，请确保你的应用请求读取扩展对象的权限。</span><span class="sxs-lookup"><span data-stu-id="77856-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77856-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="77856-122">Request headers</span></span>

| <span data-ttu-id="77856-123">名称</span><span class="sxs-lookup"><span data-stu-id="77856-123">Name</span></span>      |<span data-ttu-id="77856-124">说明</span><span class="sxs-lookup"><span data-stu-id="77856-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="77856-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="77856-125">Authorization</span></span> | <span data-ttu-id="77856-126">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="77856-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="77856-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="77856-127">Request body</span></span>

<span data-ttu-id="77856-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77856-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77856-129">响应</span><span class="sxs-lookup"><span data-stu-id="77856-129">Response</span></span>

<span data-ttu-id="77856-130">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [claimsMappingPolicy](../resources/claimsmappingpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="77856-130">If successful, this method returns a `200 OK` response code and the requested [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="77856-131">示例</span><span class="sxs-lookup"><span data-stu-id="77856-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77856-132">请求</span><span class="sxs-lookup"><span data-stu-id="77856-132">Request</span></span>

<span data-ttu-id="77856-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="77856-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="77856-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="77856-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="77856-135">C#</span><span class="sxs-lookup"><span data-stu-id="77856-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77856-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77856-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77856-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77856-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77856-138">Java</span><span class="sxs-lookup"><span data-stu-id="77856-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-claimsmappingpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77856-139">响应</span><span class="sxs-lookup"><span data-stu-id="77856-139">Response</span></span>

<span data-ttu-id="77856-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="77856-140">The following is an example of the response.</span></span>

> <span data-ttu-id="77856-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="77856-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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

