---
title: 列出 accessPackages
description: 检索 accessPackage 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1123897bca41f3d90b3b002dcab6428533141a95
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439810"
---
# <a name="list-accesspackages"></a><span data-ttu-id="ab796-103">列出 accessPackages</span><span class="sxs-lookup"><span data-stu-id="ab796-103">List accessPackages</span></span>

<span data-ttu-id="ab796-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab796-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab796-105">检索 [accessPackage 对象](../resources/accesspackage.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="ab796-105">Retrieve a list of [accessPackage](../resources/accesspackage.md) objects.</span></span>  <span data-ttu-id="ab796-106">生成的列表包括调用方有权访问的所有目录读取的所有访问包。</span><span class="sxs-lookup"><span data-stu-id="ab796-106">The resulting list includes all the access packages that the caller has access to read, across all catalogs.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab796-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ab796-107">Permissions</span></span>

<span data-ttu-id="ab796-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab796-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab796-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab796-110">Permission type</span></span>                        | <span data-ttu-id="ab796-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab796-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ab796-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab796-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab796-113">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab796-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ab796-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab796-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab796-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab796-115">Not supported.</span></span> |
| <span data-ttu-id="ab796-116">Application</span><span class="sxs-lookup"><span data-stu-id="ab796-116">Application</span></span>                            | <span data-ttu-id="ab796-117">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab796-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab796-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab796-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab796-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ab796-119">Optional query parameters</span></span>

<span data-ttu-id="ab796-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ab796-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ab796-121">例如，若要检索每个访问包的访问包策略，请添加 `$expand=accessPackageAssignmentPolicies` 。</span><span class="sxs-lookup"><span data-stu-id="ab796-121">For example, to retrieve the access package policies for each access package, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="ab796-122">若要搜索具有特定名称的访问包，请包含筛选器，如 `$filter=contains(tolower(displayName),'team')` 在查询中。</span><span class="sxs-lookup"><span data-stu-id="ab796-122">To search for access packages with a particular name, include a filter such as `$filter=contains(tolower(displayName),'team')` in the query.</span></span> <span data-ttu-id="ab796-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ab796-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab796-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab796-124">Request headers</span></span>

| <span data-ttu-id="ab796-125">名称</span><span class="sxs-lookup"><span data-stu-id="ab796-125">Name</span></span>      |<span data-ttu-id="ab796-126">说明</span><span class="sxs-lookup"><span data-stu-id="ab796-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab796-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab796-127">Authorization</span></span> | <span data-ttu-id="ab796-128">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="ab796-128">Bearer \{token\}.</span></span> <span data-ttu-id="ab796-129">必需。</span><span class="sxs-lookup"><span data-stu-id="ab796-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab796-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab796-130">Request body</span></span>

<span data-ttu-id="ab796-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab796-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab796-132">响应</span><span class="sxs-lookup"><span data-stu-id="ab796-132">Response</span></span>

<span data-ttu-id="ab796-133">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [accessPackage](../resources/accesspackage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ab796-133">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab796-134">示例</span><span class="sxs-lookup"><span data-stu-id="ab796-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab796-135">请求</span><span class="sxs-lookup"><span data-stu-id="ab796-135">Request</span></span>

<span data-ttu-id="ab796-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ab796-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab796-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab796-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackages"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
```
# <a name="c"></a>[<span data-ttu-id="ab796-138">C#</span><span class="sxs-lookup"><span data-stu-id="ab796-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab796-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab796-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab796-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab796-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab796-141">Java</span><span class="sxs-lookup"><span data-stu-id="ab796-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ab796-142">响应</span><span class="sxs-lookup"><span data-stu-id="ab796-142">Response</span></span>

<span data-ttu-id="ab796-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ab796-143">The following is an example of the response.</span></span>

> <span data-ttu-id="ab796-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ab796-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
      "description":"Sample access package",
      "displayName":"Access package for testing",
      "isHidden":false,
      "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
      "isRoleScopesVisible":false,
      "createdDateTime":"2019-01-27T18:19:50.74Z",
      "modifiedDateTime":"2019-01-27T18:19:50.74Z",
      "createdBy":"TestGA@example.com",
      "modifiedBy":"TestGA@example.com"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


