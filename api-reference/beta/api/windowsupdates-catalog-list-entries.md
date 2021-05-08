---
title: 列表条目
description: 从目录中获取 catalogEntry 资源列表。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 3a3b8903011cb5abcdeb55726f1b332730de8bb9
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241410"
---
# <a name="list-entries"></a><span data-ttu-id="b72b6-103">列表条目</span><span class="sxs-lookup"><span data-stu-id="b72b6-103">List entries</span></span>
<span data-ttu-id="b72b6-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="b72b6-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b72b6-105">从目录获取 [catalogEntry](../resources/windowsupdates-catalogentry.md) 资源 [的列表](../resources/windowsupdates-catalog.md)。</span><span class="sxs-lookup"><span data-stu-id="b72b6-105">Get a list of [catalogEntry](../resources/windowsupdates-catalogentry.md) resources from the [catalog](../resources/windowsupdates-catalog.md).</span></span>

<span data-ttu-id="b72b6-106">目前，此操作返回 [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) 或 [qualityUpdateCatalog](../resources/windowsupdates-qualityupdatecatalogentry.md) 类型的条目，继承自 **catalogEntry**。</span><span class="sxs-lookup"><span data-stu-id="b72b6-106">Currently, this operation returns entries of the [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) or [qualityUpdateCatalog](../resources/windowsupdates-qualityupdatecatalogentry.md) types, inherited from **catalogEntry**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b72b6-107">权限</span><span class="sxs-lookup"><span data-stu-id="b72b6-107">Permissions</span></span>
<span data-ttu-id="b72b6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b72b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b72b6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b72b6-110">Permission type</span></span>|<span data-ttu-id="b72b6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b72b6-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b72b6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b72b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b72b6-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b72b6-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="b72b6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b72b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b72b6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b72b6-115">Not supported.</span></span>|
|<span data-ttu-id="b72b6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b72b6-116">Application</span></span>|<span data-ttu-id="b72b6-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b72b6-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b72b6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b72b6-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/catalog/entries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b72b6-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b72b6-119">Optional query parameters</span></span>
<span data-ttu-id="b72b6-120">此方法支持一些 [OData 查询](/graph/query-parameters) 参数来帮助自定义响应，包括 `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="b72b6-120">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="b72b6-121">若要对不是从 **catalogEntry** 继承的属性使用查询参数，请包含属性的完整资源类型。</span><span class="sxs-lookup"><span data-stu-id="b72b6-121">To use a query parameter on a property that is not inherited from **catalogEntry**, include the full resource type for the property.</span></span> <span data-ttu-id="b72b6-122">例如，若要筛选 [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md)**的版本属性**，请使用 `$filter=microsoft.graph.windowsUpdates.featureUpdateCatalogEntry/version` 。</span><span class="sxs-lookup"><span data-stu-id="b72b6-122">For example, to filter on the **version** property of [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md), use `$filter=microsoft.graph.windowsUpdates.featureUpdateCatalogEntry/version`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b72b6-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b72b6-123">Request headers</span></span>
|<span data-ttu-id="b72b6-124">名称</span><span class="sxs-lookup"><span data-stu-id="b72b6-124">Name</span></span>|<span data-ttu-id="b72b6-125">说明</span><span class="sxs-lookup"><span data-stu-id="b72b6-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b72b6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b72b6-126">Authorization</span></span>|<span data-ttu-id="b72b6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b72b6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b72b6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b72b6-129">Request body</span></span>
<span data-ttu-id="b72b6-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b72b6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b72b6-131">响应</span><span class="sxs-lookup"><span data-stu-id="b72b6-131">Response</span></span>

<span data-ttu-id="b72b6-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` catalogEntry 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b72b6-132">If successful, this method returns a `200 OK` response code and a collection of catalogEntry objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b72b6-133">示例</span><span class="sxs-lookup"><span data-stu-id="b72b6-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b72b6-134">请求</span><span class="sxs-lookup"><span data-stu-id="b72b6-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b72b6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b72b6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_catalogentry"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries
```
# <a name="c"></a>[<span data-ttu-id="b72b6-136">C#</span><span class="sxs-lookup"><span data-stu-id="b72b6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-catalogentry-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b72b6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b72b6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-catalogentry-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b72b6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b72b6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-catalogentry-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b72b6-139">Java</span><span class="sxs-lookup"><span data-stu-id="b72b6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-catalogentry-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b72b6-140">响应</span><span class="sxs-lookup"><span data-stu-id="b72b6-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.catalogEntry)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
      "id": "c1dec151-c151-c1de-51c1-dec151c1dec1",
      "displayName": "String",
      "releaseDateTime": "String (timestamp)",
      "deployableUntilDateTime": "String (timestamp)",
      "version": "String"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
      "id": "d0c03fbb-43b9-4dff-840b-974ef227384d",
      "displayName": "String",
      "releaseDateTime": "String (timestamp)",
      "deployableUntilDateTime": "String (timestamp)",
      "isExpeditable": true,
      "qualityUpdateClassification": "security"
    }
  ]
}
```

