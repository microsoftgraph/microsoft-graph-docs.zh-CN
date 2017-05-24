# <a name="section-resource-type"></a>section 资源类型

OneNote 笔记本中的分区。分区可包含页面。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|识别创建项目的用户、设备和应用程序。只读。|
|createdDateTime|DateTimeOffset|分区的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。|
|id|String|分区的唯一标识符。只读。|
|isDefault|Boolean|指示其是否是用户的默认分区。只读。|
|lastModifiedBy|[identitySet](identityset.md)|识别创建项目的用户、设备和应用程序。只读。|
|lastModifiedDateTime|DateTimeOffset|上次修改分区的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。|
|links|[SectionLinks](sectionlinks.md)|用于打开分区的链接。如果安装了 OneNote 本机客户端，则 `oneNoteClientURL` 链接将在其中打开分区。`oneNoteWebURL` 将在 OneNote Online 中打开分区。|
|displayName|String|分区名称。 |
|pagesUrl|String|可以在其中获取分区中所有页面的详细信息的 `pages` 终结点。只读。|
|self|String|可以在其中获取关于分区的详细信息的终结点。只读。|

## <a name="relationships"></a>关系
| 关系 | 类型    |说明|
|:---------------|:--------|:----------|
|pages|[Page](page.md) collection|分区中的页面集合。只读。可为 NULL。|
|parentNotebook|[Notebook](notebook.md)|包含分区的笔记本。只读。|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|包含分区的分区组。只读。|

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get section](../api/section_get.md) | [Section](section.md) |读取分区的属性和关系。|
|[Create page](../api/section_post_pages.md) |[Page](page.md)| 通过发布到指定分区中的页面集合创建页面。|
|[List pages](../api/section_list_pages.md) |[Page](page.md) collection| 获取指定分区中的页面集合。|
|[copyToNotebook](../api/section_copytonotebook.md)|无|将分区复制到特定笔记本。|
|[copyToSectionGroup](../api/section_copytosectiongroup.md)|无|将分区复制到特定分区组。|


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
