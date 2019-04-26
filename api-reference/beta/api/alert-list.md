---
title: 列出警报
description: 检索警报对象的列表。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: ab9ec3c42b0a46279e43660e241fb3cde52e83a9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322684"
---
# <a name="list-alerts"></a><span data-ttu-id="6d80d-103">列出警报</span><span class="sxs-lookup"><span data-stu-id="6d80d-103">List alerts</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d80d-104">检索[警报](../resources/alert.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="6d80d-104">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d80d-105">权限</span><span class="sxs-lookup"><span data-stu-id="6d80d-105">Permissions</span></span>

<span data-ttu-id="6d80d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d80d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d80d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d80d-108">Permission type</span></span>      | <span data-ttu-id="6d80d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d80d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d80d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d80d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="6d80d-111">securityevents.readwrite.all、securityevents.readwrite.all 和所有</span><span class="sxs-lookup"><span data-stu-id="6d80d-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="6d80d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d80d-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6d80d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d80d-113">Not supported.</span></span>  |
|<span data-ttu-id="6d80d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d80d-114">Application</span></span> | <span data-ttu-id="6d80d-115">securityevents.readwrite.all、securityevents.readwrite.all 和所有</span><span class="sxs-lookup"><span data-stu-id="6d80d-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d80d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d80d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d80d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6d80d-117">Optional query parameters</span></span>

<span data-ttu-id="6d80d-118">此方法支持以下[OData 查询参数](/graph/query-parameters)来帮助自定义响应:</span><span class="sxs-lookup"><span data-stu-id="6d80d-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="6d80d-119">`$top`将返回每个安全 API 提供程序的聚合顶级结果。</span><span class="sxs-lookup"><span data-stu-id="6d80d-119">`$top` will return the aggregated top results from each security API provider.</span></span>

<span data-ttu-id="6d80d-120">若要返回其他属性集, 请使用 OData `$select`查询参数指定所需的一组**警报**属性。</span><span class="sxs-lookup"><span data-stu-id="6d80d-120">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="6d80d-121">例如, 若要返回 "**分配给**"、"**类别**" 和 "**严重性**" 属性, 请将`$select=assignedTo,category,severity`以下内容添加到您的查询中:。</span><span class="sxs-lookup"><span data-stu-id="6d80d-121">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="6d80d-122">**注意:**`$top`的警报限制为1000个, 并且组合`$top`  +  `$skip`不能超过6000个警报。</span><span class="sxs-lookup"><span data-stu-id="6d80d-122">**Note:** `$top` has a limit of 1000 alerts, and a combination of `$top` + `$skip` cannot exceed 6000 alerts.</span></span> <span data-ttu-id="6d80d-123">例如, `/security/alerts?$top=10&$skip=5990`将返回`200 OK`响应代码, 但`/security/alerts?$top=10&$skip=5991`将返回`400 Bad Request`响应代码。</span><span class="sxs-lookup"><span data-stu-id="6d80d-123">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>  <span data-ttu-id="6d80d-124">有关详细信息, 请参阅[Microsoft Graph 安全 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="6d80d-124">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d80d-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d80d-125">Request headers</span></span>

| <span data-ttu-id="6d80d-126">名称</span><span class="sxs-lookup"><span data-stu-id="6d80d-126">Name</span></span>      |<span data-ttu-id="6d80d-127">说明</span><span class="sxs-lookup"><span data-stu-id="6d80d-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6d80d-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d80d-128">Authorization</span></span>  | <span data-ttu-id="6d80d-129">持有者 {代码}。</span><span class="sxs-lookup"><span data-stu-id="6d80d-129">Bearer {code}.</span></span> <span data-ttu-id="6d80d-130">必填。</span><span class="sxs-lookup"><span data-stu-id="6d80d-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d80d-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d80d-131">Request body</span></span>

<span data-ttu-id="6d80d-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6d80d-132">Do not supply a request body for this method.</span></span> <span data-ttu-id="6d80d-133">请求正文将被忽略。</span><span class="sxs-lookup"><span data-stu-id="6d80d-133">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="6d80d-134">响应</span><span class="sxs-lookup"><span data-stu-id="6d80d-134">Response</span></span>

<span data-ttu-id="6d80d-135">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**alert**对象集合。</span><span class="sxs-lookup"><span data-stu-id="6d80d-135">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="6d80d-136">如果从提供程序返回的状态代码或者提供程序超时, 则响应将是一个`206 Partial Content`状态代码, 提供程序的响应在警告标头中。</span><span class="sxs-lookup"><span data-stu-id="6d80d-136">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="6d80d-137">有关详细信息, 请参阅[Microsoft Graph 安全 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="6d80d-137">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="6d80d-138">示例</span><span class="sxs-lookup"><span data-stu-id="6d80d-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d80d-139">请求</span><span class="sxs-lookup"><span data-stu-id="6d80d-139">Request</span></span>

<span data-ttu-id="6d80d-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6d80d-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts
```

### <a name="response"></a><span data-ttu-id="6d80d-141">响应</span><span class="sxs-lookup"><span data-stu-id="6d80d-141">Response</span></span>

<span data-ttu-id="6d80d-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6d80d-142">The following is an example of the response.</span></span>

><span data-ttu-id="6d80d-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6d80d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
