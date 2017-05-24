# <a name="list-contracts"></a>列出 contract

检索与合作伙伴租户关联的 [contract](../resources/contract.md) 对象列表。

### <a name="prerequisites"></a>先决条件

需要以下**范围**之一才能执行此 API：*Directory.Read.All*、*Directory.ReadWrite.All* 或 *Directory.AccessAsUser.All*

### <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

### <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters)来帮助自定义响应。 

> 支持筛选 customerId、defaultDomainName 和 displayName。

### <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| 授权  | *需要*持有者&lt;令牌&gt; |

### <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

### <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contract](../resources/contract.md) 对象集合。

### <a name="example"></a>示例
##### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts
```

##### <a name="response"></a>响应

注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->