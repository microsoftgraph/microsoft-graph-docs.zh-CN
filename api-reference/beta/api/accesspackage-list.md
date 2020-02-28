---
title: 列出 accessPackages
description: 检索 accessPackage 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 660eccde7211c23bfbb6ecc44faa20532934f965
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331113"
---
# <a name="list-accesspackages"></a><span data-ttu-id="d3d25-103">列出 accessPackages</span><span class="sxs-lookup"><span data-stu-id="d3d25-103">List accessPackages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3d25-104">检索[accessPackage](../resources/accesspackage.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d3d25-104">Retrieve a list of [accessPackage](../resources/accesspackage.md) objects.</span></span>  <span data-ttu-id="d3d25-105">生成的列表包括呼叫者有权读取的所有目录中的所有 access 程序包。</span><span class="sxs-lookup"><span data-stu-id="d3d25-105">The resulting list includes all the access packages that the caller has access to read, across all catalogs.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3d25-106">权限</span><span class="sxs-lookup"><span data-stu-id="d3d25-106">Permissions</span></span>

<span data-ttu-id="d3d25-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3d25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3d25-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3d25-109">Permission type</span></span>                        | <span data-ttu-id="d3d25-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3d25-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d3d25-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3d25-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="d3d25-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3d25-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="d3d25-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3d25-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3d25-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3d25-114">Not supported.</span></span> |
| <span data-ttu-id="d3d25-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3d25-115">Application</span></span>                            | <span data-ttu-id="d3d25-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3d25-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3d25-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3d25-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3d25-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d3d25-118">Optional query parameters</span></span>

<span data-ttu-id="d3d25-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d3d25-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d3d25-120">例如，若要检索每个访问程序包的访问程序包策略，请`$expand=accessPackageAssignmentPolicies`添加。</span><span class="sxs-lookup"><span data-stu-id="d3d25-120">For example, to retrieve the access package policies for each access package, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="d3d25-121">若要搜索具有特定名称的 access 程序包，请`$filter=contains(tolower(displayName),'team')`在查询中添加筛选器（如查询）。</span><span class="sxs-lookup"><span data-stu-id="d3d25-121">To search for access packages with a particular name, include a filter such as `$filter=contains(tolower(displayName),'team')` in the query.</span></span> <span data-ttu-id="d3d25-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d3d25-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3d25-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3d25-123">Request headers</span></span>

| <span data-ttu-id="d3d25-124">名称</span><span class="sxs-lookup"><span data-stu-id="d3d25-124">Name</span></span>      |<span data-ttu-id="d3d25-125">说明</span><span class="sxs-lookup"><span data-stu-id="d3d25-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d3d25-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3d25-126">Authorization</span></span> | <span data-ttu-id="d3d25-127">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="d3d25-127">Bearer \{token\}.</span></span> <span data-ttu-id="d3d25-128">必填。</span><span class="sxs-lookup"><span data-stu-id="d3d25-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3d25-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3d25-129">Request body</span></span>

<span data-ttu-id="d3d25-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d3d25-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3d25-131">响应</span><span class="sxs-lookup"><span data-stu-id="d3d25-131">Response</span></span>

<span data-ttu-id="d3d25-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackage](../resources/accesspackage.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d3d25-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3d25-133">示例</span><span class="sxs-lookup"><span data-stu-id="d3d25-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3d25-134">请求</span><span class="sxs-lookup"><span data-stu-id="d3d25-134">Request</span></span>

<span data-ttu-id="d3d25-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d3d25-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3d25-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3d25-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackages"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
```
# <a name="c"></a>[<span data-ttu-id="d3d25-137">C#</span><span class="sxs-lookup"><span data-stu-id="d3d25-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3d25-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3d25-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3d25-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3d25-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3d25-140">响应</span><span class="sxs-lookup"><span data-stu-id="d3d25-140">Response</span></span>

<span data-ttu-id="d3d25-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d3d25-141">The following is an example of the response.</span></span>

> <span data-ttu-id="d3d25-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d3d25-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
