# <a name="list-alerts"></a><span data-ttu-id="14c96-101">列出 alerts</span><span class="sxs-lookup"><span data-stu-id="14c96-101">List alerts</span></span>

<span data-ttu-id="14c96-102">检索 [alert](../resources/alert.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="14c96-102">Retrieve a list of nameditem objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="14c96-103">权限</span><span class="sxs-lookup"><span data-stu-id="14c96-103">Permissions</span></span>

<span data-ttu-id="14c96-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="14c96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="14c96-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="14c96-106">Permission type</span></span>      | <span data-ttu-id="14c96-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14c96-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14c96-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14c96-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="14c96-109">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14c96-109">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="14c96-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14c96-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="14c96-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="14c96-111">Not supported.</span></span>  |
|<span data-ttu-id="14c96-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="14c96-112">Application</span></span> | <span data-ttu-id="14c96-113">SecurityEvents.Read.All、SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14c96-113">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14c96-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14c96-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14c96-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="14c96-115">Optional query parameters</span></span>

<span data-ttu-id="14c96-116">此方法支持以下 [OData 查询参数](../../../concepts/query_parameters.md)以帮助自定义响应：</span><span class="sxs-lookup"><span data-stu-id="14c96-116">This method supports the following [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="14c96-117">`$top` 将从每个安全 API 提供程序返回聚合的顶级结果。</span><span class="sxs-lookup"><span data-stu-id="14c96-117">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="14c96-118">若要返回替代属性集，请使用 OData `$select`查询参数指定所需的 **alert** 属性集。</span><span class="sxs-lookup"><span data-stu-id="14c96-118">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="14c96-119">例如，若要返回 **assignedTo**、**category**和 **severity** 属性，请将以下内容添加到您的查询中：`$select=assignedTo,category,severity`。</span><span class="sxs-lookup"><span data-stu-id="14c96-119">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14c96-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="14c96-120">Request headers</span></span>

| <span data-ttu-id="14c96-121">名称</span><span class="sxs-lookup"><span data-stu-id="14c96-121">Name</span></span>      |<span data-ttu-id="14c96-122">说明</span><span class="sxs-lookup"><span data-stu-id="14c96-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="14c96-123">授权</span><span class="sxs-lookup"><span data-stu-id="14c96-123">Authorization</span></span>  | <span data-ttu-id="14c96-p103">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="14c96-p103">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="14c96-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="14c96-126">Request body</span></span>

<span data-ttu-id="14c96-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="14c96-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="14c96-128">请求正文将被忽略。</span><span class="sxs-lookup"><span data-stu-id="14c96-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="14c96-129">响应</span><span class="sxs-lookup"><span data-stu-id="14c96-129">Response</span></span>

<span data-ttu-id="14c96-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 **alert** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="14c96-130">If successful, this method returns a `200 OK` response code and collection of **Attachment** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14c96-131">示例</span><span class="sxs-lookup"><span data-stu-id="14c96-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="14c96-132">请求</span><span class="sxs-lookup"><span data-stu-id="14c96-132">Request</span></span>

<span data-ttu-id="14c96-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="14c96-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```

### <a name="response"></a><span data-ttu-id="14c96-134">响应</span><span class="sxs-lookup"><span data-stu-id="14c96-134">Response</span></span>

<span data-ttu-id="14c96-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="14c96-135">The following is an example of the response.</span></span>

><span data-ttu-id="14c96-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="14c96-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
