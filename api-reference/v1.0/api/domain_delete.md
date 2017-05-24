# <a name="delete-domain"></a>删除域

从租户中删除域。

> **重要说明：**
> - 已删除的域不可恢复。<br />
> - 如果存在任何仍旧依赖域的资源或对象，尝试删除会失败。可以通过使用此 [列出 domainNameReferences](domain_list_domainnamereferences.md) API 查找所有从属的资源。

### <a name="prerequisites"></a>先决条件

要执行此 API，需要以下**范围**之一：*Domain.ReadWrite.All* 或 *Directory.AccessAsUser.All*

### <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> 对于 {id}，请使用其完全限定的域名指定该域。

### <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:---------------|:----------|
| 授权  | *需要*持有者&lt;令牌&gt; |
| Content-Type  | application/json |

### <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

### <a name="response"></a>响应

如果成功，此方法返回 `204, No Content` 响应代码。它不返回响应正文。

### <a name="example"></a>示例
##### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/V1.0/domains/contoso.com
```

##### <a name="response"></a>响应

注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->