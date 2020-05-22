---
title: 列出 accessPackageCatalogs
description: 检索 accessPackageCatalog 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 729d7504fc7cfffcb80f763f7b6c428e90b4bf31
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345427"
---
# <a name="list-accesspackagecatalogs"></a><span data-ttu-id="9d85d-103">列出 accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="9d85d-103">List accessPackageCatalogs</span></span>

<span data-ttu-id="9d85d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d85d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d85d-105">检索[accessPackageCatalog](../resources/accesspackagecatalog.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9d85d-105">Retrieve a list of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d85d-106">权限</span><span class="sxs-lookup"><span data-stu-id="9d85d-106">Permissions</span></span>

<span data-ttu-id="9d85d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d85d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d85d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d85d-109">Permission type</span></span>                        | <span data-ttu-id="9d85d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d85d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9d85d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d85d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d85d-112">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="9d85d-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9d85d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d85d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d85d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d85d-114">Not supported.</span></span> |
| <span data-ttu-id="9d85d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d85d-115">Application</span></span>                            | <span data-ttu-id="9d85d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d85d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d85d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d85d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d85d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9d85d-118">Optional query parameters</span></span>

<span data-ttu-id="9d85d-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9d85d-119">This method supports some of the OData query parameters to help customize the response.</span></span>  <span data-ttu-id="9d85d-120">例如，若要检索每个目录中的访问包，请 `$expand=accessPackages` 在查询中加入。</span><span class="sxs-lookup"><span data-stu-id="9d85d-120">For example, to retrieve the access packages in each catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="9d85d-121">若要搜索具有特定名称的 access 程序包目录，请 `$filter=contains(tolower(displayName),'staff')` 在查询中包含筛选器。</span><span class="sxs-lookup"><span data-stu-id="9d85d-121">To search for access package catalogs with a particular name, include a filter such as `$filter=contains(tolower(displayName),'staff')` in the query.</span></span>  <span data-ttu-id="9d85d-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9d85d-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d85d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d85d-123">Request headers</span></span>

| <span data-ttu-id="9d85d-124">名称</span><span class="sxs-lookup"><span data-stu-id="9d85d-124">Name</span></span>      |<span data-ttu-id="9d85d-125">说明</span><span class="sxs-lookup"><span data-stu-id="9d85d-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9d85d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d85d-126">Authorization</span></span> | <span data-ttu-id="9d85d-127">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="9d85d-127">Bearer \{token\}.</span></span> <span data-ttu-id="9d85d-128">必填。</span><span class="sxs-lookup"><span data-stu-id="9d85d-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d85d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d85d-129">Request body</span></span>

<span data-ttu-id="9d85d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9d85d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d85d-131">响应</span><span class="sxs-lookup"><span data-stu-id="9d85d-131">Response</span></span>

<span data-ttu-id="9d85d-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[accessPackageCatalog](../resources/accesspackagecatalog.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="9d85d-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9d85d-133">示例</span><span class="sxs-lookup"><span data-stu-id="9d85d-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9d85d-134">请求</span><span class="sxs-lookup"><span data-stu-id="9d85d-134">Request</span></span>

<span data-ttu-id="9d85d-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9d85d-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9d85d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d85d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalogs"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs
```
# <a name="c"></a>[<span data-ttu-id="9d85d-137">C#</span><span class="sxs-lookup"><span data-stu-id="9d85d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d85d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d85d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d85d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d85d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9d85d-140">响应</span><span class="sxs-lookup"><span data-stu-id="9d85d-140">Response</span></span>

<span data-ttu-id="9d85d-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9d85d-141">The following is an example of the response.</span></span>

> <span data-ttu-id="9d85d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9d85d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
