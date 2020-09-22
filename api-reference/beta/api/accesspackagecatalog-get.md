---
title: 获取 accessPackageCatalog
description: 检索 accesspackagecatalog 对象的属性和关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d18ce4e203cb3ab066736cb3c8a86c7d7609feef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983744"
---
# <a name="get-accesspackagecatalog"></a><span data-ttu-id="71b3a-103">获取 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="71b3a-103">Get accessPackageCatalog</span></span>

<span data-ttu-id="71b3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71b3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71b3a-105">检索 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71b3a-105">Retrieve the properties and relationships of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="71b3a-106">权限</span><span class="sxs-lookup"><span data-stu-id="71b3a-106">Permissions</span></span>

<span data-ttu-id="71b3a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71b3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71b3a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="71b3a-109">Permission type</span></span>                        | <span data-ttu-id="71b3a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71b3a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="71b3a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71b3a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="71b3a-112">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="71b3a-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="71b3a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71b3a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71b3a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="71b3a-114">Not supported.</span></span> |
| <span data-ttu-id="71b3a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="71b3a-115">Application</span></span>                            | <span data-ttu-id="71b3a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="71b3a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71b3a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71b3a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71b3a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="71b3a-118">Optional query parameters</span></span>

<span data-ttu-id="71b3a-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="71b3a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="71b3a-120">例如，若要检索目录中的访问包，请 `$expand=accessPackages` 在查询中加入。</span><span class="sxs-lookup"><span data-stu-id="71b3a-120">For example, to retrieve the access packages in a catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="71b3a-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="71b3a-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="71b3a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="71b3a-122">Request headers</span></span>

| <span data-ttu-id="71b3a-123">名称</span><span class="sxs-lookup"><span data-stu-id="71b3a-123">Name</span></span>      |<span data-ttu-id="71b3a-124">说明</span><span class="sxs-lookup"><span data-stu-id="71b3a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71b3a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="71b3a-125">Authorization</span></span> | <span data-ttu-id="71b3a-126">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="71b3a-126">Bearer \{token\}.</span></span> <span data-ttu-id="71b3a-127">必需。</span><span class="sxs-lookup"><span data-stu-id="71b3a-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71b3a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="71b3a-128">Request body</span></span>

<span data-ttu-id="71b3a-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71b3a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71b3a-130">响应</span><span class="sxs-lookup"><span data-stu-id="71b3a-130">Response</span></span>

<span data-ttu-id="71b3a-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="71b3a-131">If successful, this method returns a `200 OK` response code and the requested [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71b3a-132">示例</span><span class="sxs-lookup"><span data-stu-id="71b3a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="71b3a-133">请求</span><span class="sxs-lookup"><span data-stu-id="71b3a-133">Request</span></span>

<span data-ttu-id="71b3a-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="71b3a-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71b3a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="71b3a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalog"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```
# <a name="c"></a>[<span data-ttu-id="71b3a-136">C#</span><span class="sxs-lookup"><span data-stu-id="71b3a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71b3a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71b3a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71b3a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71b3a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="71b3a-139">响应</span><span class="sxs-lookup"><span data-stu-id="71b3a-139">Response</span></span>

<span data-ttu-id="71b3a-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="71b3a-140">The following is an example of the response.</span></span>

> <span data-ttu-id="71b3a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="71b3a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


