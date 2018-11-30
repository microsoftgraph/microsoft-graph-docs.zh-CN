---
title: 列出警报
description: 检索警报对象的列表。
ms.openlocfilehash: c25784f62d37722fc997e57b9f15c9857133b964
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010395"
---
# <a name="list-alerts"></a><span data-ttu-id="a864c-103">列出警报</span><span class="sxs-lookup"><span data-stu-id="a864c-103">List alerts</span></span>

<span data-ttu-id="a864c-104">检索[通知](../resources/alert.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a864c-104">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a864c-105">权限</span><span class="sxs-lookup"><span data-stu-id="a864c-105">Permissions</span></span>

<span data-ttu-id="a864c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a864c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a864c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a864c-108">Permission type</span></span>      | <span data-ttu-id="a864c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a864c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a864c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a864c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a864c-111">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a864c-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="a864c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a864c-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a864c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a864c-113">Not supported.</span></span>  |
|<span data-ttu-id="a864c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a864c-114">Application</span></span> | <span data-ttu-id="a864c-115">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a864c-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a864c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a864c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a864c-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a864c-117">Optional query parameters</span></span>

<span data-ttu-id="a864c-118">此方法支持以下[OData 查询参数](/graph/query-parameters)以帮助自定义响应：</span><span class="sxs-lookup"><span data-stu-id="a864c-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="a864c-119">`$top`将返回从每个安全 API 提供程序的聚合的顶级结果。</span><span class="sxs-lookup"><span data-stu-id="a864c-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="a864c-120">若要返回替代属性集，请使用 OData`$select`查询参数指定的所需的**通知**属性集。</span><span class="sxs-lookup"><span data-stu-id="a864c-120">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="a864c-121">例如，若要返回**assignedTo**、**类别**和**严重性**属性，请添加以下到您的查询： `$select=assignedTo,category,severity`。</span><span class="sxs-lookup"><span data-stu-id="a864c-121">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a864c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a864c-122">Request headers</span></span>

| <span data-ttu-id="a864c-123">名称</span><span class="sxs-lookup"><span data-stu-id="a864c-123">Name</span></span>      |<span data-ttu-id="a864c-124">说明</span><span class="sxs-lookup"><span data-stu-id="a864c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a864c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a864c-125">Authorization</span></span>  | <span data-ttu-id="a864c-p103">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="a864c-p103">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a864c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a864c-128">Request body</span></span>

<span data-ttu-id="a864c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a864c-129">Do not supply a request body for this method.</span></span> <span data-ttu-id="a864c-130">在请求正文将被忽略。</span><span class="sxs-lookup"><span data-stu-id="a864c-130">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="a864c-131">响应</span><span class="sxs-lookup"><span data-stu-id="a864c-131">Response</span></span>

<span data-ttu-id="a864c-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的**通知**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="a864c-132">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="a864c-133">如果从提供程序返回状态代码之外的 2xx 或 404 或提供程序超时，如果响应将`206 Partial Content`与提供程序响应警告标头中的状态代码。</span><span class="sxs-lookup"><span data-stu-id="a864c-133">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the providers response in a warning header.</span></span> <span data-ttu-id="a864c-134">有关详细信息，请参阅[Microsoft Graph 安全 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="a864c-134">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="a864c-135">示例</span><span class="sxs-lookup"><span data-stu-id="a864c-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="a864c-136">请求</span><span class="sxs-lookup"><span data-stu-id="a864c-136">Request</span></span>

<span data-ttu-id="a864c-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a864c-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```

### <a name="response"></a><span data-ttu-id="a864c-138">响应</span><span class="sxs-lookup"><span data-stu-id="a864c-138">Response</span></span>

<span data-ttu-id="a864c-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a864c-139">The following is an example of the response.</span></span>

><span data-ttu-id="a864c-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a864c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
