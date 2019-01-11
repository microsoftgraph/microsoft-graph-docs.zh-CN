---
title: 列出警报
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 6036514c2aeabe287fd019ce69157d4b7897af60
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860205"
---
# <a name="list-alerts"></a><span data-ttu-id="88fe4-104">列出警报</span><span class="sxs-lookup"><span data-stu-id="88fe4-104">List alerts</span></span>

 > <span data-ttu-id="88fe4-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="88fe4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88fe4-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="88fe4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="88fe4-107">检索[通知](../resources/alert.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="88fe4-107">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="88fe4-108">权限</span><span class="sxs-lookup"><span data-stu-id="88fe4-108">Permissions</span></span>

<span data-ttu-id="88fe4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88fe4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88fe4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="88fe4-111">Permission type</span></span>      | <span data-ttu-id="88fe4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88fe4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88fe4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88fe4-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="88fe4-114">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88fe4-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="88fe4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88fe4-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="88fe4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88fe4-116">Not supported.</span></span>  |
|<span data-ttu-id="88fe4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="88fe4-117">Application</span></span> | <span data-ttu-id="88fe4-118">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88fe4-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88fe4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88fe4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88fe4-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="88fe4-120">Optional query parameters</span></span>

<span data-ttu-id="88fe4-121">此方法支持以下[OData 查询参数](/graph/query-parameters)以帮助自定义响应：</span><span class="sxs-lookup"><span data-stu-id="88fe4-121">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="88fe4-122">`$top`将返回从每个安全 API 提供程序的聚合的顶级结果。</span><span class="sxs-lookup"><span data-stu-id="88fe4-122">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="88fe4-123">若要返回替代属性集，请使用 OData`$select`查询参数指定的所需的**通知**属性集。</span><span class="sxs-lookup"><span data-stu-id="88fe4-123">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="88fe4-124">例如，若要返回**assignedTo**、**类别**和**严重性**属性，请添加以下到您的查询： `$select=assignedTo,category,severity`。</span><span class="sxs-lookup"><span data-stu-id="88fe4-124">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="88fe4-125">**注意：**`$top`的限制为 1000年警报和组合`$top`  +  `$skip`不能超过 6000 通知。</span><span class="sxs-lookup"><span data-stu-id="88fe4-125">**Note:** `$top` has a limit of 1000 alerts, and a combination of `$top` + `$skip` cannot exceed 6000 alerts.</span></span> <span data-ttu-id="88fe4-126">例如，`/security/alerts?$top=10&$skip=5990`会返回`200 OK`响应代码，但`/security/alerts?$top=10&$skip=5991`将返回`400 Bad Request`响应代码。</span><span class="sxs-lookup"><span data-stu-id="88fe4-126">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>  <span data-ttu-id="88fe4-127">有关详细信息，请参阅[Microsoft Graph 安全 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="88fe4-127">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="88fe4-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="88fe4-128">Request headers</span></span>

| <span data-ttu-id="88fe4-129">名称</span><span class="sxs-lookup"><span data-stu-id="88fe4-129">Name</span></span>      |<span data-ttu-id="88fe4-130">说明</span><span class="sxs-lookup"><span data-stu-id="88fe4-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="88fe4-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="88fe4-131">Authorization</span></span>  | <span data-ttu-id="88fe4-p106">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="88fe4-p106">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88fe4-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="88fe4-134">Request body</span></span>

<span data-ttu-id="88fe4-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88fe4-135">Do not supply a request body for this method.</span></span> <span data-ttu-id="88fe4-136">在请求正文将被忽略。</span><span class="sxs-lookup"><span data-stu-id="88fe4-136">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="88fe4-137">响应</span><span class="sxs-lookup"><span data-stu-id="88fe4-137">Response</span></span>

<span data-ttu-id="88fe4-138">如果成功，此方法返回`200 OK`响应代码和响应正文中的**通知**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="88fe4-138">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="88fe4-139">如果从提供程序返回状态代码之外的 2xx 或 404 或提供程序超时，如果响应将`206 Partial Content`与警告标头中的提供程序的响应状态代码。</span><span class="sxs-lookup"><span data-stu-id="88fe4-139">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="88fe4-140">有关详细信息，请参阅[Microsoft Graph 安全 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="88fe4-140">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="88fe4-141">示例</span><span class="sxs-lookup"><span data-stu-id="88fe4-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="88fe4-142">请求</span><span class="sxs-lookup"><span data-stu-id="88fe4-142">Request</span></span>

<span data-ttu-id="88fe4-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="88fe4-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts
```

### <a name="response"></a><span data-ttu-id="88fe4-144">响应</span><span class="sxs-lookup"><span data-stu-id="88fe4-144">Response</span></span>

<span data-ttu-id="88fe4-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="88fe4-145">The following is an example of the response.</span></span>

><span data-ttu-id="88fe4-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="88fe4-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
