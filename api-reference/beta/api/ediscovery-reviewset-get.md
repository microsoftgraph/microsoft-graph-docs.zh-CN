---
title: 获取 reviewSet
description: 检索 reviewSet 对象的属性和关系。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 220a52d7ceb7a3b5fce766a9ec98dbe9c7bf308b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044695"
---
# <a name="get-reviewset"></a><span data-ttu-id="638d6-103">获取 reviewSet</span><span class="sxs-lookup"><span data-stu-id="638d6-103">Get reviewSet</span></span>

<span data-ttu-id="638d6-104">命名空间：microsoft.graph.ediscovery.ediscovery</span><span class="sxs-lookup"><span data-stu-id="638d6-104">Namespace: microsoft.graph.ediscovery.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="638d6-105">检索 [reviewSet](../resources/ediscovery-reviewset.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="638d6-105">Retrieve the properties and relationships of a [reviewSet](../resources/ediscovery-reviewset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="638d6-106">权限</span><span class="sxs-lookup"><span data-stu-id="638d6-106">Permissions</span></span>

<span data-ttu-id="638d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="638d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="638d6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="638d6-109">Permission type</span></span>|<span data-ttu-id="638d6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="638d6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="638d6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="638d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="638d6-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="638d6-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="638d6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="638d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="638d6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="638d6-114">Not supported.</span></span>|
|<span data-ttu-id="638d6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="638d6-115">Application</span></span>|<span data-ttu-id="638d6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="638d6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="638d6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="638d6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="638d6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="638d6-118">Optional query parameters</span></span>

<span data-ttu-id="638d6-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="638d6-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="638d6-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="638d6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="638d6-121">默认情况下，将返回所有审阅集字段;但是，您可以使用 OData 查询参数指定要返回 `$select` 的某些字段。</span><span class="sxs-lookup"><span data-stu-id="638d6-121">By default, all review set fields are returned; however, you can specify certain fields to return using the OData `$select` query parameter.</span></span>  <span data-ttu-id="638d6-122">例如，若要仅返回 **displayName** 和 ID，请向查询中添加以下内容 `$select=displayName,Id` ：。</span><span class="sxs-lookup"><span data-stu-id="638d6-122">For example, to only return the **displayName** and ID, add the following to your query: `$select=displayName,Id`.</span></span>

<span data-ttu-id="638d6-123">由于请求可能会返回许多情况，因此可以使用 **displayName 筛选它们**。</span><span class="sxs-lookup"><span data-stu-id="638d6-123">Because a request can return many cases, you can filter them by using **displayName**.</span></span>  <span data-ttu-id="638d6-124">若要按 **displayName 进行筛选**，请向查询中添加以下内容：，其中 `$filter=displayName eq 'rs1'` 审阅集名称为 rs1。</span><span class="sxs-lookup"><span data-stu-id="638d6-124">To filter by **displayName**, add the following to your query: `$filter=displayName eq 'rs1'`, where the review set name is rs1.</span></span>

<span data-ttu-id="638d6-125">有关筛选和指定字段的信息，请参阅在 [OData URI 中使用筛选器表达式 ](/dynamics-nav/using-filter-expressions-in-odata-uris)。</span><span class="sxs-lookup"><span data-stu-id="638d6-125">For more information about filtering and specifying fields, see [Using Filter Expressions in OData URIs ](/dynamics-nav/using-filter-expressions-in-odata-uris).</span></span>

## <a name="request-headers"></a><span data-ttu-id="638d6-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="638d6-126">Request headers</span></span>

| <span data-ttu-id="638d6-127">名称</span><span class="sxs-lookup"><span data-stu-id="638d6-127">Name</span></span>      |<span data-ttu-id="638d6-128">说明</span><span class="sxs-lookup"><span data-stu-id="638d6-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="638d6-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="638d6-129">Authorization</span></span> | <span data-ttu-id="638d6-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="638d6-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="638d6-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="638d6-132">Request body</span></span>

<span data-ttu-id="638d6-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="638d6-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="638d6-134">响应</span><span class="sxs-lookup"><span data-stu-id="638d6-134">Response</span></span>

<span data-ttu-id="638d6-135">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="638d6-135">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="638d6-136">示例</span><span class="sxs-lookup"><span data-stu-id="638d6-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="638d6-137">请求</span><span class="sxs-lookup"><span data-stu-id="638d6-137">Request</span></span>

<span data-ttu-id="638d6-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="638d6-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="638d6-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="638d6-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reviewset"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets/0157910c-57ce-4e48-bd4b-90f3c88ca32e
```
# <a name="c"></a>[<span data-ttu-id="638d6-140">C#</span><span class="sxs-lookup"><span data-stu-id="638d6-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="638d6-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="638d6-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="638d6-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="638d6-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="638d6-143">Java</span><span class="sxs-lookup"><span data-stu-id="638d6-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reviewset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="638d6-144">响应</span><span class="sxs-lookup"><span data-stu-id="638d6-144">Response</span></span>

<span data-ttu-id="638d6-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="638d6-145">The following is an example of the response.</span></span>

> <span data-ttu-id="638d6-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="638d6-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d')/reviewSets/$entity",
    "id": "0157910c-57ce-4e48-bd4b-90f3c88ca32e",
    "displayName": "My Reviewset 3",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-11T08:40:14.9486058Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get reviewSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
