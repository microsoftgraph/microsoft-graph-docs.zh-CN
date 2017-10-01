# <a name="recentnotebook-resource-type"></a>recentNotebook 资源类型

最近访问过的 OneNote 笔记本。 **recentNotebook** 类似于 [notebook](notebook.md)，不同之处在于属性较少。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|名称|字符串|笔记本的名称。|
|lastAccessedTime|DateTimeOffset|上次修改笔记本的日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。|
|links|[recentNotebookLinks](recentnotebooklinks.md)|用于打开笔记本的链接。 `oneNoteClientURL` 链接可以在 OneNote 客户端（如果已安装的话）中打开笔记本。 `oneNoteWebURL` 链接可以在 OneNote Online 中打开笔记本。|
|sourceService|String|笔记本驻留的后端存储，可以是 `OneDriveForBusiness` 或 `OneDrive`。|

## <a name="json-representation"></a>JSON 表示形式

下面是此资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebook"
}-->

```json
{
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.recentNotebookLinks"},
  "sourceService": "String"
}

```

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[getRecentNotebooks](../api/notebook_getrecentnotebooks.md) | [notebook](notebook.md) 集合 | 获取用户最近访问过的一组笔记本。 |
