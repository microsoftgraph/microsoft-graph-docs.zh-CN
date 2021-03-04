---
title: 获取 accessPackageCatalog
description: 检索 accesspackagecatalog 对象的属性和关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bae6156db7160d860975d1642bb75d51bbea8909
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439588"
---
# <a name="get-accesspackagecatalog"></a><span data-ttu-id="df65e-103">获取 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="df65e-103">Get accessPackageCatalog</span></span>

<span data-ttu-id="df65e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df65e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df65e-105">检索 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="df65e-105">Retrieve the properties and relationships of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="df65e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="df65e-106">Permissions</span></span>

<span data-ttu-id="df65e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df65e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df65e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="df65e-109">Permission type</span></span>                        | <span data-ttu-id="df65e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df65e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="df65e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df65e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="df65e-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df65e-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="df65e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df65e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df65e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="df65e-114">Not supported.</span></span> |
| <span data-ttu-id="df65e-115">Application</span><span class="sxs-lookup"><span data-stu-id="df65e-115">Application</span></span>                            | <span data-ttu-id="df65e-116">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df65e-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df65e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df65e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="df65e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="df65e-118">Optional query parameters</span></span>

<span data-ttu-id="df65e-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="df65e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="df65e-120">例如，若要检索目录中的访问包，请包括在 `$expand=accessPackages` 查询中。</span><span class="sxs-lookup"><span data-stu-id="df65e-120">For example, to retrieve the access packages in a catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="df65e-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="df65e-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="df65e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="df65e-122">Request headers</span></span>

| <span data-ttu-id="df65e-123">名称</span><span class="sxs-lookup"><span data-stu-id="df65e-123">Name</span></span>      |<span data-ttu-id="df65e-124">说明</span><span class="sxs-lookup"><span data-stu-id="df65e-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="df65e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="df65e-125">Authorization</span></span> | <span data-ttu-id="df65e-126">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="df65e-126">Bearer \{token\}.</span></span> <span data-ttu-id="df65e-127">必需。</span><span class="sxs-lookup"><span data-stu-id="df65e-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df65e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="df65e-128">Request body</span></span>

<span data-ttu-id="df65e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="df65e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df65e-130">响应</span><span class="sxs-lookup"><span data-stu-id="df65e-130">Response</span></span>

<span data-ttu-id="df65e-131">如果成功，此方法在响应正文中返回响应代码和请求的 `200 OK` [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df65e-131">If successful, this method returns a `200 OK` response code and the requested [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df65e-132">示例</span><span class="sxs-lookup"><span data-stu-id="df65e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df65e-133">请求</span><span class="sxs-lookup"><span data-stu-id="df65e-133">Request</span></span>

<span data-ttu-id="df65e-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="df65e-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="df65e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="df65e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalog"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```
# <a name="c"></a>[<span data-ttu-id="df65e-136">C#</span><span class="sxs-lookup"><span data-stu-id="df65e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df65e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df65e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df65e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df65e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df65e-139">Java</span><span class="sxs-lookup"><span data-stu-id="df65e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackagecatalog-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="df65e-140">响应</span><span class="sxs-lookup"><span data-stu-id="df65e-140">Response</span></span>

<span data-ttu-id="df65e-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="df65e-141">The following is an example of the response.</span></span>

> <span data-ttu-id="df65e-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="df65e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


