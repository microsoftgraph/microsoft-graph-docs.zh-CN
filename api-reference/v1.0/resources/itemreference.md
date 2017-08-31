# <a name="itemreference-resource-type"></a>ItemReference 资源类型

**ItemReference** 资源提供了通过 API 查找 [DriveItem](driveitem.md) 的必要信息。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a>属性

| 属性      | 类型                              | 说明                                                                                                |
| :------------ | :-------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| driveId       | 字符串                            | 包含项的驱动器实例的唯一标识符。只读。                                 |
| id            | String                            | 项在驱动器中的唯一标识符。只读。                                                     |
| name          | 字符串                            | 所引用的项的名称。只读。                                                          |
| 路径          | String                            | 可用于导航到该项的路径。只读。                                                  |
| shareId       | String                            | 可通过 [Shares](../api/shares_get.md) API 访问共享资源的唯一标识符。 |
| sharepointIds | [sharepointIds](sharepointids.md) | 返回对 SharePoint REST 兼容性有用的标识符。只读。                                   |

## <a name="remarks"></a>注解

为了从 **itemReference** 资源中找到 **driveItem**，请构建以下格式的 URL：

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

**path** 值是相对于目标驱动器的 API 路径，例如：`/drive/root:/Documents/myfile.docx`。

要检索人工可读路径中的痕迹，可以放心地忽略路径字符串中的第一个 `:` 之前的所有内容。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
