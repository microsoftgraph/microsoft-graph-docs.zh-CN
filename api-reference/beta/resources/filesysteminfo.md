# <a name="filesysteminfo-resource-type"></a>FileSystemInfo 资源类型

 **FileSystemInfo** 资源包含设备本地文件系统所报告的项目本地版本的属性。和在本地设备上一样，此 facet 可用于指定项目的上次修改日期或创建日期。

**注意：****FileSystemInfo** 属性不可用于 SharePoint 中的 DriveItems 或 OneDrive for Business。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "lastAccessedDateTime"
  ],
  "@odata.type": "microsoft.graph.fileSystemInfo"
}-->

```json
{
  "createdDateTime": "datetime",
  "lastModifiedDateTime": "datetime"
}
```

## <a name="properties"></a>属性

| 属性                 | 类型           | 说明                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| **createdDateTime**      | DateTimeOffset | 在客户端创建文件时的 UTC 日期和时间。                                                              |
| **lastAccessedDateTime** | DateTimeOffset | 上次访问文件时的 UTC 日期和时间。仅可用于[最近的文件列表](../api/drive_recent.md)。 |
| **lastModifiedDateTime** | DateTimeOffset | 在客户端上次修改文件时的 UTC 日期和时间。                                                        |

## <a name="notes"></a>注释

来自 [DriveItem](driveitem.md) 资源上同一属性的 **createdDateTime** 和 **lastModifiedDateTime** 值有所不同。DriveItem 资源上的值是从服务中所见的创建和修改的日期和时间。**FileSystemInfo** 资源中存储的值由客户端提供。

例如，如果星期一在设备上创建文件，但直到星期二才上载到服务，则上载文件的客户端应写入 `fileSystemInfo` facet，以包括星期一这一创建日期。检索项元数据时，项的创建日期将反映为星期二，但 `fileSystemInfo` facet 将显示星期一这一创建的原始创建日期。

这些属性为读/写。如果正在上载文件，并且知道这些字段的本地客户端值，则应该在请求中包括它们。

如果文件内容已更新且未提供这些属性，**lastModifiedDateTime** 将自动重置为当前时间。

## <a name="remarks"></a>注解

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSystemInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
