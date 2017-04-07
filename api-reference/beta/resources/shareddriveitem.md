# <a name="shareddriveitem-resource-type"></a>SharedDriveItem 资源类型

使用 [Shares](../api/shares_get.md) API 访问共享的 [DriveItem](driveitem.md) 时，返回 **SharedDriveItem** 资源。该资源类似于 [Drive](drive.md) 资源，但仅限于可通过共享链接或 shareId 访问的 DriveItems。

### <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->
```json
{
    "id": "string",
    "name": "string",
    "owner": { "@odata.type": "microsoft.graph.identitySet" },
    "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
    "root": { "@odata.type": "microsoft.graph.driveItem" }
}
```

### <a name="properties"></a>属性

| 属性  | 类型                                  | 说明                                                          |
|:----------|:--------------------------------------|:---------------------------------------------------------------------|
| id        | String                                | 要访问的内容的唯一标识符。                  |
| 名称      | String                                | 共享项的显示名称。                                 |
| 所有者     | [IdentitySet](identityset.md)         | 正在引用的共享项的所有者信息。     |
| 项目     | Collection([DriveItem](driveitem.md)) | 共享的 DriveItem 资源的集合。不能枚举该集合，但可以通过其唯一 ID 访问项。 |
| root      | [DriveItem](driveitem.md)             | 顶级共享 DriveItem。如果共享单个文件，则此项是文件。如果共享文件夹，则此项将是文件夹。可以使用项的 facet 确定要应用的服务案例。 |

## <a name="remarks"></a>注解 

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharepointIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->