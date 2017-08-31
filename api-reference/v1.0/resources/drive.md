# <a name="drive-resource-type"></a>驱动器资源类型

驱动器资源是表示用户的 OneDrive 或 SharePoint 中文档库的顶级对象。

OneDrive 用户必须始终具有至少一个可用驱动器，即默认驱动器。没有 OneDrive 许可证的用户不能拥有可用的默认驱动器。

## <a name="json-representation"></a>JSON 表示形式

下面是**驱动器**资源的 JSON 表示形式。

**驱动器**资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "items", "root", "special", "owner", "description" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "id": "string (identifier)",
  "driveType": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "root": {"@odata.type": "microsoft.graph.driveItem" },
  "items": [ {"@odata.type": "microsoft.graph.driveItem" }],
  "special": [ {"@odata.type": "microsoft.graph.driveItem" }],

  /* inherited from baseItem */
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a>属性

| 属性             | 类型                          | 说明                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | String                        | 驱动器唯一标识符。只读。                                                                                                                                                                                   |
| createdBy            | [identitySet][]               | 识别创建项目的用户、设备或应用程序。只读。                                                                                                                                                  |
| createdDateTime      | dateTimeOffset                | 创建项的日期和时间。只读。                                                                                                                                                                                       |
| driveType            | String                        | 说明了由该资源表示的驱动器的类型。OneDrive 个人版驱动器将返回 `personal`。OneDrive for Business 将返回 `business`。SharePoint 文档库将返回 `documentLibrary`。只读。 |
| lastModifiedBy       | [identitySet][]               | 上次修改项目的用户、设备和应用程序的标识。只读。                                                                                                                                           |
| lastModifiedDateTime | dateTimeOffset                | 上次修改项目的日期和时间。只读。                                                                                                                                                                             |
| name                 | string                        | 项目名称。读写。                                                                                                                                                                                                |
| 所有者                | [identitySet](identityset.md) | 可选。拥有此驱动器的用户帐户。只读。                                                                                                                                                                       |
| 配额                | [配额](quota.md)             | 可选。有关驱动器的存储空间配额的信息。只读。                                                                                                                                                          |
| sharepointIds        | [sharepointIds][]             | 返回对 SharePoint REST 兼容性有用的标识符。只读。                                                                                                                                                         |
| webUrl               | string (url)                  | 在浏览器中显示此资源的 URL。只读。                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md

## <a name="relationships"></a>关系

| 关系 | 类型                                 | 说明                                                              |
| :----------- | :----------------------------------- | :----------------------------------------------------------------------- |
| 项目        | [driveitem](driveitem.md) 集合 | 驱动器中包含的所有项。只读。可为 NULL。                   |
| 根         | [driveitem](driveitem.md)            | 驱动器的根文件夹。只读。                                 |
| special      | [driveitem](driveitem.md) 集合 | OneDrive 中可用的公用文件夹的集合。只读。可为 Null。 |

## <a name="methods"></a>方法

下列方法均可用于驱动器资源。

| 方法                                                | REST 路径                        |
| :---------------------------------------------------- | :------------------------------- |
| [获取用户的默认驱动器](../api/drive_get.md)       | `GET /me/drive`                  |
| [获取其他用户的驱动器](../api/drive_get.md)       | `GET /users/{user-id}/drive`     |
| [获取驱动器的根文件夹](../api/item_get.md)     | `GET /drives/{drive-id}/root`    |
| [列出驱动器中的项目](../api/item_list_children.md) | `GET /me/drive/root/children`    |
| [列出驱动器中的更改](../api/item_delta.md)       | `GET /me/drive/root/delta`       |
| [搜索驱动器中的项目](../api/item_search.md)      | `GET /me/drive/search(q='text')` |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "drive resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive"
}-->
