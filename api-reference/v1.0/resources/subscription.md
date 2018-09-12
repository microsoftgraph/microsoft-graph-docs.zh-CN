# <a name="subscription-resource-type"></a>订阅资源类型

借助订阅，客户端应用可以接收 Microsoft Graph 中的数据更改的通知。 目前，已为下列资源启用了订阅：

- Outlook 中的邮件、活动和联系人
- 来自 Office 组的对话
- 来自 OneDrive 的驱动器根项
- 来自 Azure Active Directory 用户和组

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscription",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false,
        "sortable": false
      }
    }
  ]
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| changeType | 字符串 | 必需。 指示订阅资源中将引发通知的更改类型。 支持的值是：`created`、`updated`、`deleted`。 可以使用以逗号分隔的列表组合多个值。<br><br>注意：驱动器根项通知仅支持 `updated` changeType。 用户和组通知支持 `updated` 和 `deleted` changeType。|
| notificationUrl | 字符串 | 必需。 将接收通知的端点的 URL。 此 URL 必须使用 HTTPS 协议。 |
| resource | 字符串 | 必需。 指定将监视其是否发生更改的资源。 不包含基 URL (`https://graph.microsoft.com/v1.0/`)。 |
| expirationDateTime | [dateTime](http://tools.ietf.org/html/rfc3339) | 必需。 指定 webhook 订阅过期的日期和时间。 时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。  请参阅下表，了解支持的最长订阅有效期。 |
| clientState | 字符串 | 可选。 指定服务为每个通知发送的 `clientState` 属性的值。 最大长度为 128 个字符。 通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。 |
| id | 字符串 | 订阅的唯一标识符。只读。 |
| applicationId | 字符串 | 用于创建订阅的应用程序的标识符。 只读。 |
| creatorId | 字符串 | 用户或创建订阅的服务主体的标识符。 如果应用程序使用委派权限创建订阅，此字段包含应用程序调用代表登录用户的 id。 如果应用程序使用应用程序权限，此字段包含应用程序对应的服务主体的 id。 只读。 |

## <a name="maximum-length-of-subscription-per-resource-type"></a>每个资源类型的最长订阅有效期

| 资源            | 最大过期时间  |
|:--------------------|:-------------------------|
| 邮件                | 4230 分钟 （3 天内）    |
| 日历            | 4230 分钟 （3 天内）    |
| 联系人            | 4230 分钟 （3 天内）    |
| 组对话 | 4230 分钟 （3 天内）    |
| 驱动器根项    | 4230 分钟 （3 天内）    |

> **注意：** 现有和新的应用都不得超过支持的值。 将来，任何超出最大值的订阅创建或续订请求都将失败。

## <a name="relationships"></a>关系

无

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-------|:------------|:------------|
| [创建订阅](../api/subscription_post_subscriptions.md) | [订阅](subscription.md) | 订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。 |
| [更新订阅](../api/subscription_update.md) | [订阅](subscription.md) | 通过更新其过期时间来续订订阅。 |
| [订阅列表](../api/subscription_list.md) | [订阅](subscription.md) | 列出了活动订阅。 |
| [获取订阅](../api/subscription_get.md) | [订阅](subscription.md) | 读取 subscription 对象的属性和关系。 |
| [删除订阅](../api/subscription_delete.md) | 无 |删除订阅对象。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
