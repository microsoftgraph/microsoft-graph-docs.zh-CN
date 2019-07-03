---
title: 列出警报
description: 检索警报对象列表。
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: 37fa0c35d0995370fac4a2d463d3d44b9adad705
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443859"
---
# <a name="list-alerts"></a><span data-ttu-id="70d17-103">列出警报</span><span class="sxs-lookup"><span data-stu-id="70d17-103">List alerts</span></span>

<span data-ttu-id="70d17-104">检索[警报](../resources/alert.md)对象列表。</span><span class="sxs-lookup"><span data-stu-id="70d17-104">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="70d17-105">权限</span><span class="sxs-lookup"><span data-stu-id="70d17-105">Permissions</span></span>

<span data-ttu-id="70d17-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70d17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70d17-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="70d17-108">Permission type</span></span>      | <span data-ttu-id="70d17-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70d17-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70d17-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70d17-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="70d17-111">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70d17-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="70d17-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70d17-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="70d17-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="70d17-113">Not supported.</span></span>  |
|<span data-ttu-id="70d17-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="70d17-114">Application</span></span> | <span data-ttu-id="70d17-115">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70d17-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70d17-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70d17-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70d17-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="70d17-117">Optional query parameters</span></span>

<span data-ttu-id="70d17-118">此方法支持以下 [OData 查询参数](/graph/query-parameters)，它们有助于自定义响应：</span><span class="sxs-lookup"><span data-stu-id="70d17-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="70d17-119">`$top` 将返回每个安全 API 提供程序的顶部聚合结果。</span><span class="sxs-lookup"><span data-stu-id="70d17-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="70d17-120">若要返回其他属性，使用 OData `$select` 查询参数指定你想要的一组 **alert** 属性。</span><span class="sxs-lookup"><span data-stu-id="70d17-120">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="70d17-121">例如，若要返回 **assignedTo**、**category** 和 **severity** 属性，向查询添加以下项：`$select=assignedTo,category,severity`。</span><span class="sxs-lookup"><span data-stu-id="70d17-121">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="70d17-122">**注意：**`$top` 的限制为 1000 条警报，`$top` + `$skip` 的组合不能超过 6000 条警报。</span><span class="sxs-lookup"><span data-stu-id="70d17-122">**Note:** `$top` has a limit of 1000 alerts, and a combination of `$top` + `$skip` cannot exceed 6000 alerts.</span></span> <span data-ttu-id="70d17-123">例如，`/security/alerts?$top=10&$skip=5990` 将返回 `200 OK` 响应代码，但 `/security/alerts?$top=10&$skip=5991` 将返回 `400 Bad Request` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="70d17-123">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>  <span data-ttu-id="70d17-124">有关详细信息，请参阅 [Microsoft Graph 安全性 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="70d17-124">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="70d17-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="70d17-125">Request headers</span></span>

| <span data-ttu-id="70d17-126">名称</span><span class="sxs-lookup"><span data-stu-id="70d17-126">Name</span></span>      |<span data-ttu-id="70d17-127">说明</span><span class="sxs-lookup"><span data-stu-id="70d17-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="70d17-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="70d17-128">Authorization</span></span>  | <span data-ttu-id="70d17-129">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="70d17-129">Bearer {code}.</span></span> <span data-ttu-id="70d17-130">必需。</span><span class="sxs-lookup"><span data-stu-id="70d17-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70d17-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="70d17-131">Request body</span></span>

<span data-ttu-id="70d17-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="70d17-132">Do not supply a request body for this method.</span></span> <span data-ttu-id="70d17-133">将忽略请求正文。</span><span class="sxs-lookup"><span data-stu-id="70d17-133">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="70d17-134">响应</span><span class="sxs-lookup"><span data-stu-id="70d17-134">Response</span></span>

<span data-ttu-id="70d17-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 **alert** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="70d17-135">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="70d17-136">如果从提供程序返回了 2xx 或 404 以外的状态代码，或者提供程序超时，则响应将是 `206 Partial Content` 状态代码，提供程序的响应位于警告标头中。</span><span class="sxs-lookup"><span data-stu-id="70d17-136">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="70d17-137">有关详细信息，请参阅 [Microsoft Graph 安全性 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="70d17-137">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="70d17-138">示例</span><span class="sxs-lookup"><span data-stu-id="70d17-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="70d17-139">请求</span><span class="sxs-lookup"><span data-stu-id="70d17-139">Request</span></span>

<span data-ttu-id="70d17-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="70d17-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="70d17-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="70d17-141">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70d17-142">C#</span><span class="sxs-lookup"><span data-stu-id="70d17-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70d17-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="70d17-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70d17-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70d17-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="70d17-145">响应</span><span class="sxs-lookup"><span data-stu-id="70d17-145">Response</span></span>

<span data-ttu-id="70d17-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="70d17-146">The following is an example of the response.</span></span>

><span data-ttu-id="70d17-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="70d17-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
