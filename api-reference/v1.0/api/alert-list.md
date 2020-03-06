---
title: 列出警报
description: 检索警报对象列表。
author: preetikr
localization_priority: Priority
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: be594c14612e8957e052ba536a1cf3c74fe7cdf6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518957"
---
# <a name="list-alerts"></a><span data-ttu-id="21ad5-103">列出警报</span><span class="sxs-lookup"><span data-stu-id="21ad5-103">List alerts</span></span>

<span data-ttu-id="21ad5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21ad5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="21ad5-105">检索[警报](../resources/alert.md)对象列表。</span><span class="sxs-lookup"><span data-stu-id="21ad5-105">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="21ad5-106">权限</span><span class="sxs-lookup"><span data-stu-id="21ad5-106">Permissions</span></span>

<span data-ttu-id="21ad5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21ad5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21ad5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="21ad5-109">Permission type</span></span>      | <span data-ttu-id="21ad5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="21ad5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21ad5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21ad5-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="21ad5-112">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21ad5-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="21ad5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21ad5-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="21ad5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="21ad5-114">Not supported.</span></span>  |
|<span data-ttu-id="21ad5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="21ad5-115">Application</span></span> | <span data-ttu-id="21ad5-116">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21ad5-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21ad5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21ad5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}' and {property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21ad5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="21ad5-118">Optional query parameters</span></span>

<span data-ttu-id="21ad5-119">此方法支持以下 [OData 查询参数](/graph/query-parameters)，它们有助于自定义响应：</span><span class="sxs-lookup"><span data-stu-id="21ad5-119">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="21ad5-120">`$top` 将返回每个安全 API 提供程序的顶部聚合结果。</span><span class="sxs-lookup"><span data-stu-id="21ad5-120">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="21ad5-121">若要返回其他属性，使用 OData `$select` 查询参数指定你想要的一组 **alert** 属性。</span><span class="sxs-lookup"><span data-stu-id="21ad5-121">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="21ad5-122">例如，若要返回 **assignedTo**、**category** 和 **severity** 属性，向查询添加以下项：`$select=assignedTo,category,severity`。</span><span class="sxs-lookup"><span data-stu-id="21ad5-122">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="21ad5-123">**注意：**`$top` OData 查询参数具有 1000 个警报的限制。</span><span class="sxs-lookup"><span data-stu-id="21ad5-123">**Note:** The `$top` OData query parameter has a limit of 1000 alerts.</span></span> <span data-ttu-id="21ad5-124">建议你在第一个 GET 查询中仅包括 `$top`，而不包括 `$skip`。</span><span class="sxs-lookup"><span data-stu-id="21ad5-124">We recommend that you include only `$top` and not `$skip` in your first GET query.</span></span> <span data-ttu-id="21ad5-125">可使用 `@odata.nextLink` 进行分页。</span><span class="sxs-lookup"><span data-stu-id="21ad5-125">You can use `@odata.nextLink` for pagination.</span></span> <span data-ttu-id="21ad5-126">如果需要使用 `$skip`，它具有 500 个警报的限制。</span><span class="sxs-lookup"><span data-stu-id="21ad5-126">If you need to use `$skip`, it has a limit of 500 alerts.</span></span> <span data-ttu-id="21ad5-127">例如，`/security/alerts?$top=10&$skip=500` 将返回 `200 OK` 响应代码，但 `/security/alerts?$top=10&$skip=501` 将返回 `400 Bad Request` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="21ad5-127">For example, `/security/alerts?$top=10&$skip=500` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=501` will return a `400 Bad Request` response code.</span></span> <span data-ttu-id="21ad5-128">有关详细信息，请参阅 [Microsoft Graph 安全性 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="21ad5-128">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="21ad5-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="21ad5-129">Request headers</span></span>

| <span data-ttu-id="21ad5-130">名称</span><span class="sxs-lookup"><span data-stu-id="21ad5-130">Name</span></span>      |<span data-ttu-id="21ad5-131">说明</span><span class="sxs-lookup"><span data-stu-id="21ad5-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="21ad5-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="21ad5-132">Authorization</span></span>  | <span data-ttu-id="21ad5-133">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="21ad5-133">Bearer {code}.</span></span> <span data-ttu-id="21ad5-134">必需。</span><span class="sxs-lookup"><span data-stu-id="21ad5-134">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="21ad5-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="21ad5-135">Request body</span></span>

<span data-ttu-id="21ad5-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="21ad5-136">Do not supply a request body for this method.</span></span> <span data-ttu-id="21ad5-137">将忽略请求正文。</span><span class="sxs-lookup"><span data-stu-id="21ad5-137">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="21ad5-138">响应</span><span class="sxs-lookup"><span data-stu-id="21ad5-138">Response</span></span>

<span data-ttu-id="21ad5-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 **alert** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="21ad5-139">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="21ad5-140">如果从提供程序返回了 2xx 或 404 以外的状态代码，或者提供程序超时，则响应将是 `206 Partial Content` 状态代码，提供程序的响应位于警告标头中。</span><span class="sxs-lookup"><span data-stu-id="21ad5-140">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="21ad5-141">有关详细信息，请参阅 [Microsoft Graph 安全性 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="21ad5-141">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="21ad5-142">示例</span><span class="sxs-lookup"><span data-stu-id="21ad5-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="21ad5-143">请求</span><span class="sxs-lookup"><span data-stu-id="21ad5-143">Request</span></span>

<span data-ttu-id="21ad5-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="21ad5-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21ad5-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="21ad5-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/alerts
```
# <a name="c"></a>[<span data-ttu-id="21ad5-146">C#</span><span class="sxs-lookup"><span data-stu-id="21ad5-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21ad5-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21ad5-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21ad5-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21ad5-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21ad5-149">Java</span><span class="sxs-lookup"><span data-stu-id="21ad5-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-alerts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="21ad5-150">响应</span><span class="sxs-lookup"><span data-stu-id="21ad5-150">Response</span></span>

<span data-ttu-id="21ad5-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="21ad5-151">The following is an example of the response.</span></span>

><span data-ttu-id="21ad5-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="21ad5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
