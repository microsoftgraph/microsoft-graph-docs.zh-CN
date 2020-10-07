---
title: 获取 reviewSet
description: 检索 reviewSet 对象的属性和关系。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 255b1c251d06414fcf625827fb1a23e00b233754
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372528"
---
# <a name="get-reviewset"></a><span data-ttu-id="23a12-103">获取 reviewSet</span><span class="sxs-lookup"><span data-stu-id="23a12-103">Get reviewSet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23a12-104">检索 [reviewSet](../resources/reviewset.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="23a12-104">Retrieve the properties and relationships of a [reviewSet](../resources/reviewset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="23a12-105">权限</span><span class="sxs-lookup"><span data-stu-id="23a12-105">Permissions</span></span>

<span data-ttu-id="23a12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23a12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23a12-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="23a12-108">Permission type</span></span>                        | <span data-ttu-id="23a12-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23a12-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="23a12-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23a12-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="23a12-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="23a12-111">User.Read</span></span> |
| <span data-ttu-id="23a12-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23a12-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23a12-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="23a12-113">Not supported.</span></span> |
| <span data-ttu-id="23a12-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="23a12-114">Application</span></span>                            | <span data-ttu-id="23a12-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="23a12-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="23a12-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23a12-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23a12-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="23a12-117">Optional query parameters</span></span>

<span data-ttu-id="23a12-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="23a12-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="23a12-119">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="23a12-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="23a12-120">默认情况下，将返回所有审阅集字段;但是，可以使用 OData 查询参数指定要返回的某些字段 `$select` 。</span><span class="sxs-lookup"><span data-stu-id="23a12-120">By default, all review set fields are returned; however, you can specify certain fields to return using the OData `$select` query parameter.</span></span>  <span data-ttu-id="23a12-121">例如，若要仅返回 **displayName** 和 ID，请在查询中添加以下内容： `$select=displayName,Id` 。</span><span class="sxs-lookup"><span data-stu-id="23a12-121">For example, to only return the **displayName** and ID, add the following to your query: `$select=displayName,Id`.</span></span>

<span data-ttu-id="23a12-122">由于请求可能会返回多种情况，因此您可以使用 **displayName**对它们进行筛选。</span><span class="sxs-lookup"><span data-stu-id="23a12-122">Because a request can return many cases, you can filter them by using **displayName**.</span></span>  <span data-ttu-id="23a12-123">若要按 **displayName**筛选，请将以下内容添加到您的查询中： `$filter=displayName eq 'rs1'` ，其中的审阅集名称为 rs1。</span><span class="sxs-lookup"><span data-stu-id="23a12-123">To filter by **displayName**, add the following to your query: `$filter=displayName eq 'rs1'`, where the review set name is rs1.</span></span>

<span data-ttu-id="23a12-124">有关筛选和指定字段的详细信息，请参阅 [在 OData uri 中使用筛选器表达式 ](/dynamics-nav/using-filter-expressions-in-odata-uris)。</span><span class="sxs-lookup"><span data-stu-id="23a12-124">For more information about filtering and specifying fields, see [Using Filter Expressions in OData URIs ](/dynamics-nav/using-filter-expressions-in-odata-uris).</span></span>

## <a name="request-headers"></a><span data-ttu-id="23a12-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="23a12-125">Request headers</span></span>

| <span data-ttu-id="23a12-126">名称</span><span class="sxs-lookup"><span data-stu-id="23a12-126">Name</span></span>      |<span data-ttu-id="23a12-127">说明</span><span class="sxs-lookup"><span data-stu-id="23a12-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="23a12-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="23a12-128">Authorization</span></span> | <span data-ttu-id="23a12-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="23a12-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23a12-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="23a12-131">Request body</span></span>

<span data-ttu-id="23a12-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="23a12-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23a12-133">响应</span><span class="sxs-lookup"><span data-stu-id="23a12-133">Response</span></span>

<span data-ttu-id="23a12-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [reviewSet](../resources/reviewset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="23a12-134">If successful, this method returns a `200 OK` response code and the requested [reviewSet](../resources/reviewset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23a12-135">示例</span><span class="sxs-lookup"><span data-stu-id="23a12-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="23a12-136">请求</span><span class="sxs-lookup"><span data-stu-id="23a12-136">Request</span></span>

<span data-ttu-id="23a12-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="23a12-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="23a12-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="23a12-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reviewset"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets/0157910c-57ce-4e48-bd4b-90f3c88ca32e
```
# <a name="c"></a>[<span data-ttu-id="23a12-139">C#</span><span class="sxs-lookup"><span data-stu-id="23a12-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23a12-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23a12-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23a12-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23a12-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="23a12-142">响应</span><span class="sxs-lookup"><span data-stu-id="23a12-142">Response</span></span>

<span data-ttu-id="23a12-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="23a12-143">The following is an example of the response.</span></span>

> <span data-ttu-id="23a12-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="23a12-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSet"
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
