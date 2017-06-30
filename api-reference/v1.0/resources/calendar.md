# <a name="calendar-resource-type"></a>日历资源类型

用作事件容器的日历。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出日历](../api/user_list_calendars.md)|[日历](calendar.md) 集合|获取所有用户的日历，或者获取默认或其他特定日历组中的日历。|
|[创建日历](../api/user_post_calendars.md) |[日历](calendar.md)| 在默认日历组或指定日历组中创建新日历。|
|[获取日历](../api/calendar_get.md) | [日历](calendar.md) |读取 calendar 对象的属性和关系。|
|[更新](../api/calendar_update.md) | [日历](calendar.md)  |更新 calendar 对象。 |
|[删除](../api/calendar_delete.md) | 无 |删除 calendar 对象。 |
|[列出 calendarView](../api/calendar_list_calendarview.md) |[事件](event.md) 集合| 从用户的主日历 `(../me/calendarview)` 或指定日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。|
|[列出事件](../api/calendar_list_events.md) |[事件](event.md) 集合| 检索日历中的事件列表。该列表包含单个实例会议和系列主控形状。|
|[创建事件](../api/calendar_post_events.md) |[事件](event.md)| 在默认或指定日历中创建新事件。|
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[日历](calendar.md)  |在新建或现有日历中创建一个或多个单值扩展属性。   |
|[获取包含单值扩展属性的日历](../api/singlevaluelegacyextendedproperty_get.md)  | [日历](calendar.md) | 通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的日历。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [日历](calendar.md) | 在新建或现有的日历中创建一个或多个多值扩展属性。  |
|[获取包含多值扩展属性的日历](../api/multivaluelegacyextendedproperty_get.md)  | [日历](calendar.md) | 使用 `$expand` 获取包含一个多值扩展属性的日历。 |


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|canEdit |Boolean |如果用户可以写入日历则为 true，否则为 false。对于创建此日历的用户，此属性为 true。此属性对于共享日历并且授予写入访问权限的用户同样为 true。 |
|canShare |Boolean |如果用户有权共享日历则为 ture，否则为 false。只有创建日历的用户才可以进行共享。 |
|canViewPrivateItems |Boolean |如果用户可以读取已标记为私有的日历项，则为 true，否则返回 false。 |
|changeKey|String|标识 calendar 对象的版本。每次日历更改时，changeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。|
|color|String|在 UI 中指定将该日历与其他日历区分开来的颜色主题。属性值有：LightBlue=0、LightGreen=1、LightOrange=2、LightGray=3、LightYellow=4、LightTeal=5、LightPink=6、LightBrown=7、LightRed=8、MaxColor=9、Auto=-1|
|id|String|组的唯一标识符。只读。|
|name|String|日历名称。|
|owner |[emailAddress](emailaddress.md) | 如果设置，则表示创建或添加日历的用户。对于用户创建或添加的日历，将 **owner** 属性设置为用户。对于与用户共享的日历，将 **owner** 属性设置为与此用户共享该日历的人员。 |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|calendarView|[事件](event.md) 集合|日历的日历视图。导航属性。只读。|
|events|[事件](event.md) 集合|日历中的事件。导航属性。只读。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为日历定义的多值扩展属性的集合。只读。可为 Null。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为日历定义的单值扩展属性的集合。只读。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendar"
}-->

```json
{
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
