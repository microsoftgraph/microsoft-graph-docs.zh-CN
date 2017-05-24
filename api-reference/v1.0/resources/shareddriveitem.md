# <a name="shareddriveitem-resource-type"></a>SharedDriveItem 资源类型

使用 [Shares](../api/shares_get.md) API 访问共享的 [driveItem](driveitem.md) 时，返回 **sharedDriveItem** 资源。

## <a name="json-representation"></a>JSON 表示形式

下面是 **sharedDriveItem** 资源的 JSON 表示形式。

**sharedDriveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。

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

    /* relationships*/
    "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
    "root": { "@odata.type": "microsoft.graph.driveItem" },
    "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
    "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a>属性

| 属性 | 类型                          | 说明                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| id       | String                        | 要访问的内容的唯一标识符。              |
| 名称     | String                        | 共享项的显示名称。                             |
| 所有者    | [IdentitySet](identityset.md) | 正在引用的共享项的所有者信息。 |

## <a name="relationships"></a>关系

| 关系 | 类型                                  | 说明                                                                                                                                                                                                |
| :----------- | :------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 项        | Collection([DriveItem](driveitem.md)) | 共享的 **driveItem** 资源的集合。不能枚举该集合，但可以通过其唯一 ID 访问项。                                                                        |
| 根         | [DriveItem](driveitem.md)             | 顶级共享 **driveItem**。如果共享单个文件，则此项是文件。如果共享文件夹，则此项将是文件夹。可以使用项的 facet 确定要应用的服务案例。 |
| driveItem    | [driveItem](driveitem.md)             | 已共享资源的 **driveItem**。这等同于**根**属性。                                                                                                             |
| 网站         | [网站](site.md)                       | 包含已共享项的**网站**资源。                                                                                                                                                |

## <a name="methods"></a>方法

| 方法                                  | REST 路径                |
| :-------------------------------------- | :----------------------- |
| [获取共享项目](../api/shares_get.md) | `GET /shares/{share-id}` |

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