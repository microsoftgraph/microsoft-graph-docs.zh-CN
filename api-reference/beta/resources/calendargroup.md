# <a name="calendargroup-resource-type"></a>calendarGroup 资源类型

一组日历。

**注意** Outlook.com 仅支持可通过 /me/calendars 快捷方式访问的默认日历组。无法删除该日历组。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出日历组](../api/user_list_calendargroups.md) |[日历](calendar.md) 集合| 获取用户的日历组。|
|[创建日历组](../api/user_post_calendargroups.md) |[日历](calendar.md)| 创建新的日历组。|
|[创建日历组](../api/calendargroup_get.md) | [calendarGroup](calendargroup.md) |读取 calendar 对象的属性和关系。|
|[更新](../api/calendargroup_update.md) | [calendarGroup](calendargroup.md) |更新 calendarGroup 对象。 |
|[删除](../api/calendargroup_delete.md) | 无 |删除 calendarGroup 对象。 |
|[列出日历](../api/calendargroup_list_calendars.md) |[日历](calendar.md) 集合| 列出日历组中的日历。|
|[创建日历](../api/calendargroup_post_calendars.md) |[日历](calendar.md)| 在日历组中创建新日历。|


## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|名称|String|组名称。|
|changeKey|String|标识日历组的版本。每次日历组更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。|
|classId|Guid|类标识符。只读。|
|id|String|组的唯一标识符。只读。|

## <a name="relationships"></a>关系
| 关系 | 类型    |说明|
|:---------------|:--------|:----------|
|日历|[日历](calendar.md) 集合|日历组中的日历。导航属性。只读。可为 Null。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendarGroup"
}-->

```json
{
  "changeKey": "string",
  "classId": "guid",
  "id": "string (identifier)",
  "name": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
