---
title: 列出 claimsMappingPolicies
description: 获取 claimsMappingPolicy 对象的列表。
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 40c3b9bc1f40634aebcc2f975d489323cd8fde50
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863286"
---
# <a name="list-claimsmappingpolicies"></a><span data-ttu-id="565c9-103">列出 claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="565c9-103">List claimsMappingPolicies</span></span>

<span data-ttu-id="565c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="565c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="565c9-105">获取[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="565c9-105">Get a list of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="565c9-106">权限</span><span class="sxs-lookup"><span data-stu-id="565c9-106">Permissions</span></span>

<span data-ttu-id="565c9-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="565c9-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="565c9-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="565c9-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="565c9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="565c9-109">Permission type</span></span>                        | <span data-ttu-id="565c9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="565c9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="565c9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="565c9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="565c9-112">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="565c9-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="565c9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="565c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="565c9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="565c9-114">Not supported.</span></span> |
| <span data-ttu-id="565c9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="565c9-115">Application</span></span>                            | <span data-ttu-id="565c9-116">Policy： Read. All，ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="565c9-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="565c9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="565c9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/claimsMappingPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="565c9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="565c9-118">Optional query parameters</span></span>

<span data-ttu-id="565c9-119">此方法支持 `$expand` 、 `$filter` `$select` 和 `$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="565c9-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="565c9-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="565c9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="565c9-121">使用时 `$expand` ，请确保您的应用程序请求读取扩展的对象的权限。</span><span class="sxs-lookup"><span data-stu-id="565c9-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="565c9-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="565c9-122">Request headers</span></span>

| <span data-ttu-id="565c9-123">名称</span><span class="sxs-lookup"><span data-stu-id="565c9-123">Name</span></span>      |<span data-ttu-id="565c9-124">说明</span><span class="sxs-lookup"><span data-stu-id="565c9-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="565c9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="565c9-125">Authorization</span></span> | <span data-ttu-id="565c9-126">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="565c9-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="565c9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="565c9-127">Request body</span></span>

<span data-ttu-id="565c9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="565c9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="565c9-129">响应</span><span class="sxs-lookup"><span data-stu-id="565c9-129">Response</span></span>

<span data-ttu-id="565c9-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="565c9-130">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="565c9-131">示例</span><span class="sxs-lookup"><span data-stu-id="565c9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="565c9-132">请求</span><span class="sxs-lookup"><span data-stu-id="565c9-132">Request</span></span>

<span data-ttu-id="565c9-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="565c9-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="565c9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="565c9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
```
# <a name="c"></a>[<span data-ttu-id="565c9-135">C#</span><span class="sxs-lookup"><span data-stu-id="565c9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-claimsmappingpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="565c9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="565c9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="565c9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="565c9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="565c9-138">Java</span><span class="sxs-lookup"><span data-stu-id="565c9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-claimsmappingpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="565c9-139">响应</span><span class="sxs-lookup"><span data-stu-id="565c9-139">Response</span></span>

<span data-ttu-id="565c9-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="565c9-140">The following is an example of the response.</span></span>

> <span data-ttu-id="565c9-141">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="565c9-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="565c9-142">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="565c9-142">All the properties will be returned from an actual call.</span></span>

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
