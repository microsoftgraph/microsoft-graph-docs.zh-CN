---
title: 列出 claimsMappingPolicies
description: 获取 claimsMappingPolicy 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b52ceec6fb0a0845500b7f34c03121cb0bdf4596
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476364"
---
# <a name="list-claimsmappingpolicies"></a><span data-ttu-id="d4504-103">列出 claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="d4504-103">List claimsMappingPolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4504-104">获取[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d4504-104">Get a list of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4504-105">权限</span><span class="sxs-lookup"><span data-stu-id="d4504-105">Permissions</span></span>

<span data-ttu-id="d4504-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4504-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4504-108">Permission type</span></span>                        | <span data-ttu-id="d4504-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4504-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d4504-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4504-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4504-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4504-111">Policy.Read.All</span></span> |
| <span data-ttu-id="d4504-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4504-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4504-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4504-113">Not supported.</span></span> |
| <span data-ttu-id="d4504-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4504-114">Application</span></span>                            | <span data-ttu-id="d4504-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4504-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4504-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4504-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/claimsMappingPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4504-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d4504-117">Optional query parameters</span></span>

<span data-ttu-id="d4504-118">`$expand`此方法支持`$filter`、 `$select`和`$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d4504-118">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="d4504-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d4504-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="d4504-120">使用`$expand`时，请确保您的应用程序请求读取扩展的对象的权限。</span><span class="sxs-lookup"><span data-stu-id="d4504-120">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4504-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4504-121">Request headers</span></span>

| <span data-ttu-id="d4504-122">名称</span><span class="sxs-lookup"><span data-stu-id="d4504-122">Name</span></span>      |<span data-ttu-id="d4504-123">说明</span><span class="sxs-lookup"><span data-stu-id="d4504-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d4504-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4504-124">Authorization</span></span> | <span data-ttu-id="d4504-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d4504-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4504-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4504-126">Request body</span></span>

<span data-ttu-id="d4504-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d4504-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4504-128">响应</span><span class="sxs-lookup"><span data-stu-id="d4504-128">Response</span></span>

<span data-ttu-id="d4504-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d4504-129">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4504-130">示例</span><span class="sxs-lookup"><span data-stu-id="d4504-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4504-131">请求</span><span class="sxs-lookup"><span data-stu-id="d4504-131">Request</span></span>

<span data-ttu-id="d4504-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d4504-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d4504-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4504-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/claimsMappingPolicies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d4504-134">C#</span><span class="sxs-lookup"><span data-stu-id="d4504-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-claimsmappingpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4504-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4504-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d4504-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4504-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d4504-137">响应</span><span class="sxs-lookup"><span data-stu-id="d4504-137">Response</span></span>

<span data-ttu-id="d4504-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d4504-138">The following is an example of the response.</span></span>

> <span data-ttu-id="d4504-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d4504-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List claimsMappingPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
