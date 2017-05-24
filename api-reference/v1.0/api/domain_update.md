# <a name="update-domain"></a>更新域

更新域对象的属性。

> **重要说明：**只有已验证的域可以进行更新。

### <a name="prerequisites"></a>先决条件

要执行此 API，需要以下**范围**之一：*Domain.ReadWrite.All* 或 *Directory.AccessAsUser.All*

### <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> 对于 {id}，请使用其完全限定的域名指定该域。

### <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| 授权  | *需要*持有者&lt;令牌&gt; |
| Content-Type  | application/json |

### <a name="request-body"></a>请求正文

在请求正文中，提供要更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，仅包含已更改的值。

### <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码，不返回任何响应正文。

### <a name="example"></a>示例
##### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/V1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->