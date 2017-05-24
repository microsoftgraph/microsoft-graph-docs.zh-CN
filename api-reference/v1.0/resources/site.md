# <a name="site-resource"></a>网站资源

**网站**资源提供 SharePoint 网站的元数据和关系。

## <a name="tasks"></a>任务

下面的所有示例都相对于 `https://graph.microsoft.com/v1.0`。

| 任务名称            | 示例请求                                   |
| :------------------- | :------------------------------------------------ |
| [获取根网站][]    | GET /sites/root                                   |
| [获取网站][]         | GET /sites/{site-id}                              |
| [根据路径获取网站][] | GET /sites/{hostname}:/{site-path}                |

[获取网站]: ../api/site_get.md
[获取根网站]: ../api/site_get.md
[根据路径获取网站]: ../api/site_get.md

## <a name="json-representation"></a>JSON 表示形式

下面是**网站**资源的 JSON 表示形式。

**driveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。

<!-- { "blockType": "resource",
       "@odata.type": "microsoft.graph.site",
       "keyProperty": "id",
       "optionalProperties": [ "root", "sharepointIds", "siteCollection", "drive", "drives", "sites" ] } -->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

## <a name="properties"></a>属性

| 属性名称            | 类型                                | 说明                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| **id**                   | string                              | 项的唯一标识符。只读。                                                  |
| **createdDateTime**      | DateTimeOffset                      | 创建项目的日期和时间。只读。                                             |
| **说明**          | string                              | 网站的描述性文本。                                                             |
| **displayName**          | string                              | 网站的完整标题。只读。                                                        |
| **lastModifiedDateTime** | DateTimeOffset                      | 上次修改项目的日期和时间。只读。                                       |
| **名称**                 | string                              | 项目名称/标题。                                                                  |
| **根**                 | [根](root.md)                     | 如果存在，则表示这是网站集中的根网站。只读。            |
| **sharepointIds**        | [sharepointIds](sharepointids.md)   | 返回对 SharePoint REST 兼容性有用的标识符。只读。                       |
| **siteCollection**       | [siteCollection](sitecollection.md) | 提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。 |
| **WebUrl**               | string (url)                        | 在浏览器中显示此项目的 URL。只读。                                          |

## <a name="relationships"></a>关系

| 关系名称 | 类型                     | 说明
|:------------------|:-------------------------|:----------------------------------
| **驱动器**         | [驱动器][]                | 此网站的默认驱动器（文档库）。
| **驱动器**        | 集合（[驱动器][]）    | 网站下方的驱动器集合（文档库）。
| **项目**         | 集合 ([baseItem][]) | 用于处理包含在此网站中的任何项目。不能枚举该集合。
| **网站**         | 集合（[网站][]）     | 网站下方的子网站的集合。

[baseItem]: baseitem.md
[驱动器]: drive.md
[identitySet]: identityset.md
[网站]: site.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Site",
  "tocBookmarks": {
    "Site": "#"
  }
} -->
