# <a name="location-resource-type"></a>位置资源类型

表示事件的位置信息。


## <a name="properties"></a>属性
| 属性  | 类型   | 说明                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| address | [physicalAddress](physicalAddress.md) |位置的街道地址。 |
| displayName  | String | 与地点相关联的名称。                       |
| locationEmailAddress | String | （可选）与地点相关联的电子邮件地址。              |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```

## <a name="remarks"></a>注解

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->