# <a name="sizerange-resource-type"></a>sizeRange 资源类型


指定传入邮件必须具有的最大大小和最小大小（以千字节为单位），以便条件或例外情况适用。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| maximumSize | Int32 | 传入邮件必须具有的最大大小（以千字节为单位），以便条件或例外情况适用。 |
| minimumSize | Int32 | 传入邮件必须具有的最小大小（以千字节为单位），以便条件或例外情况适用。 |


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->