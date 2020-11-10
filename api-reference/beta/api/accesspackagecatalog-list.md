---
title: 列出 accessPackageCatalogs
description: 检索 accessPackageCatalog 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0bae3404b27539acdb9e78fad8c165a409e34954
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951911"
---
# <a name="list-accesspackagecatalogs"></a><span data-ttu-id="20c3e-103">列出 accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="20c3e-103">List accessPackageCatalogs</span></span>

<span data-ttu-id="20c3e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20c3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20c3e-105">检索 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="20c3e-105">Retrieve a list of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="20c3e-106">权限</span><span class="sxs-lookup"><span data-stu-id="20c3e-106">Permissions</span></span>

<span data-ttu-id="20c3e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20c3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20c3e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="20c3e-109">Permission type</span></span>                        | <span data-ttu-id="20c3e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20c3e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="20c3e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20c3e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="20c3e-112">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="20c3e-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="20c3e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20c3e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20c3e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="20c3e-114">Not supported.</span></span> |
| <span data-ttu-id="20c3e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="20c3e-115">Application</span></span>                            | <span data-ttu-id="20c3e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="20c3e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20c3e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20c3e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20c3e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="20c3e-118">Optional query parameters</span></span>

<span data-ttu-id="20c3e-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="20c3e-119">This method supports some of the OData query parameters to help customize the response.</span></span>  <span data-ttu-id="20c3e-120">例如，若要检索每个目录中的访问包，请 `$expand=accessPackages` 在查询中加入。</span><span class="sxs-lookup"><span data-stu-id="20c3e-120">For example, to retrieve the access packages in each catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="20c3e-121">若要搜索具有特定名称的 access 程序包目录，请 `$filter=contains(tolower(displayName),'staff')` 在查询中包含筛选器。</span><span class="sxs-lookup"><span data-stu-id="20c3e-121">To search for access package catalogs with a particular name, include a filter such as `$filter=contains(tolower(displayName),'staff')` in the query.</span></span>  <span data-ttu-id="20c3e-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="20c3e-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="20c3e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="20c3e-123">Request headers</span></span>

| <span data-ttu-id="20c3e-124">名称</span><span class="sxs-lookup"><span data-stu-id="20c3e-124">Name</span></span>      |<span data-ttu-id="20c3e-125">说明</span><span class="sxs-lookup"><span data-stu-id="20c3e-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20c3e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="20c3e-126">Authorization</span></span> | <span data-ttu-id="20c3e-127">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="20c3e-127">Bearer \{token\}.</span></span> <span data-ttu-id="20c3e-128">必填。</span><span class="sxs-lookup"><span data-stu-id="20c3e-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20c3e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="20c3e-129">Request body</span></span>

<span data-ttu-id="20c3e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="20c3e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20c3e-131">响应</span><span class="sxs-lookup"><span data-stu-id="20c3e-131">Response</span></span>

<span data-ttu-id="20c3e-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="20c3e-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20c3e-133">示例</span><span class="sxs-lookup"><span data-stu-id="20c3e-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20c3e-134">请求</span><span class="sxs-lookup"><span data-stu-id="20c3e-134">Request</span></span>

<span data-ttu-id="20c3e-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="20c3e-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20c3e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="20c3e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalogs"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs
```
# <a name="c"></a>[<span data-ttu-id="20c3e-137">C#</span><span class="sxs-lookup"><span data-stu-id="20c3e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20c3e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20c3e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20c3e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20c3e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20c3e-140">Java</span><span class="sxs-lookup"><span data-stu-id="20c3e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackagecatalogs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="20c3e-141">响应</span><span class="sxs-lookup"><span data-stu-id="20c3e-141">Response</span></span>

<span data-ttu-id="20c3e-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="20c3e-142">The following is an example of the response.</span></span>

> <span data-ttu-id="20c3e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="20c3e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
      "description":"Sample access package catalog",
      "displayName":"Access package catalog for testing",
      "isExternallyVisible":false,
      "catalogType":"UserManaged",
      "catalogStatus":"Published",
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
  "description": "List accessPackageCatalogs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


