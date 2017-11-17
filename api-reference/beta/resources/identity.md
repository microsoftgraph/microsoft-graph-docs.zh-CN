# <a name="identity-resource-type"></a>身份资源类型

**身份**资源表示_主角_的身份。例如，主角可以是用户、设备或应用程序。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}
```

## <a name="properties"></a>属性

| 属性    | 类型   | 说明                                                                                                                                                                                                                                                                                                           |
|:------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| displayName | String | 此身份的显示名称。注意，该信息并不总是可用或最新。例如，如果用户更改了其显示名称，API 会在以后的响应中显示新值，但与用户相关联的项在使用 [delta](../api/item_delta.md) 时不会显示为更改后的值。        |
| id          | String | 身份的唯一标识符。                                                                                                                                                                                                                                                                                   |

## <a name="remarks"></a>注解

在某些情况下，角色唯一标识符可能不可用。在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
