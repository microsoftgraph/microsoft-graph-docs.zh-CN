# <a name="activity-resource-type"></a>活动资源类型

表示应用内的单一活动——例如，电视节目、文档或视频游戏中的当前活动。 当用户预订那个活动时，该预订捕获作为 [历史记录项](projectrome_historyitem.md)，显示该活动的开始和结束时间。 经过一段时间后当用户重新预订该活动时，单一用户活动会记录着多个历史记录项。

你可以在多个设备使用 Microsoft Graph 中的活动使用户能够回到他们当时在应用中正在做的事情。 你的应用所创建的活动会显示在所有用户的设备上，并以深层链接让用户接触到你应用内的特定内容。 你可以将你应用内的特定内容表示为 Windows 中展示的目的地，并且通过 Cortana 通知数在 iOS 和 Android 设备上都可以访问。

因为每个应用都不一样，所以这取决于你了解将你应用程序内的操作映射到将出现在 Cortana 和日程表中的用户活动的最佳方式。 例如，游戏可能为每个关卡创建活动、文档创作应用程序可能会为每个唯一的文档创建活动，业务线应用程序可能会为每个工作流创建活动。

用户活动将展示在用户体验的 Cortana 和 Windows 日程表中，重点以帮助用户回到他们过去从事过的内容来提高用户生产力和效率。

## <a name="methods"></a>方法

|方法 | 返回类型 | 说明|
|:------|:------------|:-----------|
|[创建或替换活动](../api/projectrome_put_activity.md) | [活动](projectrome_activity.md) |创建或替换现有的活动 (upsert)。 appActivityId 需要是 URL-safe 的（除 RFC 2396 未保留的字符外所有字符都必须转换为十六进制表示），但原始的 appActivityId 不必是 URL-safe 的。 |
|[删除活动](../api/projectrome_delete_activity.md) | 没有内容 | 从你的应用中删除那个用户的指定活动。|
|[获取活动](../api/projectrome_get_activities.md) |  [活动](projectrome_activity.md)集合 | 获取给定用户的应用的活动。|
|[获取最近的活动](../api/projectrome_get_recent_activities.md) |  [活动](projectrome_activity.md)集合 | 按照最近创建或更新的 [historyItems](projectrome_historyitem.md)排序并以此为根据来获取你给定用户的应用的最新活动。|

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|userTimezone | 字符串 | 可选。 用于生成活动的用户设备所在的时区当时位于在活动创建时；值作为 Olson ID 提供，以便支持跨平台表示形式。|
|createdDateTime | DateTimeOffset | 由服务器设置。 服务器创建对象时的 UTC DateTime。 |
|lastModifiedDateTime | DateTimeOffset | 由服务器设置。 服务器修改对象时的 UTC DateTime。 |
|ID | 字符串 | 用于 URL 寻址的服务器生成的 ID。|
|appActivityId | 字符串 | 必需。 应用环境中唯一的活动 ID——由调用程序提供并且此后是不可变的。|
|activitySourceHost | 字符串 | 必需项。 表示应用的跨平台标识映射的域的 URL。 映射或者以域托管的 JSON 文件存储，或者通过 Windows 开发人员中心配置。 JSON 文件命名为跨平台应用标识符并托管在你的 HTTPS 域的根，或者在顶级域，或者包括子域。 例如：https://contoso.com 或 https://myapp.contoso.com，但不是 https://myapp.contoso.com/somepath。 你必须每个跨平台应用标识都具有唯一文件和域 （或子域）。 例如，Word vs. PowerPoint 就需要单独的文件和域。|
|appDisplayName | 字符串 | 可选。 用于在用户的本地设备上未安装应用的情况下生成使用活动的应用的简短文本说明。|
|activationUrl | 字符串 | 必需项。 由 appId 表示的用于启动最佳本机体验的活动 URL。 如果没有本机的应用存在，则可能会启动一个基于 Web 的应用。|
|fallbackUrl | 字符串 | 可选。 用于启动基于 Web 的应用中的活动的 URL（如果可用）。|
|contentUrl | 字符串 | 可选。 用于内容可以呈现在本机或基于 Web 的应用体验之外的事件（例如，RSS 源中的项目的指针）。|
|visualElements| [visualInfo](../resources/projectrome_visualinfo.md) | 必需。 包含呈现 UX 活动信息的对象。|
|contentInfo | 无类型的 JSON 对象 | 可选。 一段自定义数据—— JSON-LD 根据 [schema.org](http://schema.org) 语法的内容的可扩展说明。|
|expirationDateTime | DateTimeOffset | 由服务器设置。 对象在服务器上过期时的 UTC DateTime。|
|状态 | 状态 | 由服务器设置。 一个用于标识有效对象的状态代码。 值：活动、已更新、已删除、已忽略。|

## <a name="relationships"></a>关系

|关系 | 类型 | 说明|
|:------------|:-----|:-----------|
|historyItems| [activityHistoryItem](../resources/projectrome_historyitem.md) 集合 | 可选。 NavigationProperty/Containment；活动的 historyItems 的导航属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "appDisplayName",
    "fallbackUrl",
    "contentUrl",
    "contentInfo",
    "visualElements",
    "historyItems"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.userActivity",
  "@odata.annotations": [
    {
      "capabilities": {
        "countable": false,
        "selectable": false,
        "skippable": false
      }
    }
  ]
}-->

```json
{
    "appActivityId": "String",
    "activitySourceHost": "String (host name/domain/URL)",
    "userTimezone": "String",
    "appDisplayName": "String",
    "activationUrl": "String (URL)",
    "contentUrl": "String (URL)",
    "fallbackUrl": "String (URL)",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "expirationDateTime": "DateTimeOffset",
    "id": "String",
    "status": "active | updated | deleted | ignored",
    "contentInfo": { "@odata.type": "microsoft.graph.Json" },
    "visualElements": { "@odata.type": "microsoft.graph.visualInfo" },
    "historyItems": [{ "@odata.type": "microsoft.graph.activityHistoryItem" }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
