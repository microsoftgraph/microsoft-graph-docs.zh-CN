# <a name="list-domainnamereferences"></a>列出 domainNameReferences

通过对域的引用检索 [directoryObject](../resources/directoryobject.md) 列表。返回列表将包含依赖域的所有目录对象。

### <a name="prerequisites"></a>先决条件

要执行此 API，需要以下**范围**之一：*Directory.Read.All* 或 *Domain.ReadWrite.All*

### <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> 对于 {id}，请使用其完全限定的域名指定该域。

### <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。

### <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| 授权  | *需要*持有者&lt;令牌&gt; |

### <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

### <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。

### <a name="example"></a>示例
##### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains/contoso.com/domainNameReferences
```

##### <a name="response"></a>响应
注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "odata.type": "Microsoft.DirectoryServices.User",
        "objectType": "User",
        "objectId": "567a0db6-289c-43f7-a650-2645c03cbbbb",
        "accountEnabled": true,
        "displayName": "TestUser1",
        "facsimileTelephoneNumber": null,
        "mailNickname": "testuser1",
        "mobile": null,
        "userPrincipalName": "testuser1@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->