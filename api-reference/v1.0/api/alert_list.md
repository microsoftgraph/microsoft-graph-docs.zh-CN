# <a name="list-alerts"></a>列出 alerts

检索 [alert](../resources/alert.md) 对象的列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  SecurityEvents.Read.All、SecurityEvents.ReadWrite.All  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | SecurityEvents.Read.All、SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持以下 [OData 查询参数](../../../concepts/query_parameters.md)以帮助自定义响应：

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- `$top` 将从每个安全 API 提供程序返回聚合的顶级结果。  

若要返回替代属性集，请使用 OData `$select`查询参数指定所需的 **alert** 属性集。  例如，若要返回 **assignedTo**、**category**和 **severity** 属性，请将以下内容添加到您的查询中：`$select=assignedTo,category,severity`。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| 授权  | Bearer {code}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。 请求正文将被忽略。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 **alert** 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```

### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
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
