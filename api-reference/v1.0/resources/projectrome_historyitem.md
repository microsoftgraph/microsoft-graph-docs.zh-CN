# <a name="historyitem-resource-type"></a>historyItem 资源类型

代表应用程序中[活动](projectrome_activity.md)的历史记录项。 用户活动代表应用程序内的单个目标——例如，电视节目、文档或视频游戏中的当前活动。 当用户参与那个活动时，将参与作为 历史记录项捕获，显示该活动的开始和结束时间。 经过一段时间后当用户重新参与该活动时，单一用户活动会记录着多个历史记录项。

当应用程序创建会话时，应将 **historyItem** 对象添加到**活动**对象以反映用户互动的时间段。 每次用户继续参与活动时，新的 **historyItem** 会添加到活动中，以累计用户的互动。

## <a name="methods"></a>方法

|方法 | 返回类型 | 说明|
|:------|:------------|:-----------|
|[创建或替换 historyItem](../api/projectrome_put_historyitem.md) | [historyItem](projectrome_historyitem.md) | 为该活动 (upsert) 创建或替换现有的 **historyItem**。 ID 必须是 GUID。|
|[删除 historyItem](../api/projectrome_delete_historyitem.md) | 没有内容 | 为该活动删除指定的 **historyItem**。|

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|状态 | 状态 | 由服务器设置。 一个用于标识有效对象的状态代码。 值：活动、已更新、已删除、已忽略。|
|userTimezone | 字符串 | 可选。 用于生成活动的用户设备所在的时区当时位于活动创建时。 值作为 Olson ID 提供，以便支持跨平台表示形式。|
|createdDateTime | DateTimeOffset | 由服务器设置。 服务器创建对象时的 UTC DateTime。|
|lastModifiedDateTime | DateTimeOffset | 由服务器设置。 在服务器上修改对象时的 UTC DateTime。|
|ID | 字符串 | 必需。  **historyItem** 对象的客户端集 GUID。|
|startedDateTime | DateTimeOffset | 必需。 启动 **historyItem** （活动会话）时的 UTC DateTime。 所需的时间线历史记录。|
|lastActiveDateTime | DateTimeOffset | 可选。 **historyItem** （活动会话）最后被理解为活动或已完成时的 UTC DateTime，如果为空，**historyItem** 状态应为“正在进行”。|
|expirationDateTime | DateTimeOffset | 可选。  **historyItem** 将进行硬删除时的 UTC DateTime。 可以由客户端设置。|
|activeDurationSeconds | int | 可选。 活动用户互动的持续时间。 如果未提供，则从 **startedDateTime** 和 **lastActiveDateTime**计算得出。|

## <a name="relationships"></a>关系

|关系 | 类型 | 说明|
|:------------|:-----|:-----------|
|activity| [userActivity](../resources/projectrome_activity.md) | 可选。 NavigationProperty/Containment；关联活动的导航属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
