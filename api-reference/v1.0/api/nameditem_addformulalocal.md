# <a name="add-named-item-formulalocal"></a>添加已命名项 FormulaLocal
使用用户的公式区域设置，将新名称添加到给定范围的集合。

## <a name="prerequisites"></a>先决条件
要执行此 API，需要以下**范围**之一：

  * Files.ReadWrite
  * Sites.Read.All
  
## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {code}|


## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数       | 类型    |说明|
|:---------------|:--------|:----------|
|name|string|已命名项的名称。|
|公式|字符串|名称将引用的公式或区域。|
|comment|字符串|与此已命名项相关联的注释。|

## <a name="response"></a>响应
如果成功，此方法将在响应正文中返回 `200, OK` 响应代码和 [NamedItem](../resources/NamedItem.md) 对象。

## <a name="example"></a>示例
下面是一个如何调用此 API 的示例。
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "myRange",
  "formula": "=A10+B10",
  "comment": "Comment for the named item"
}
```

##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "name": "myRange",
  "comment": "Sample range",
  "scope": "Workbook",
  "type": "String",
  "visible": true,
  "value": "=A10+B10"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
