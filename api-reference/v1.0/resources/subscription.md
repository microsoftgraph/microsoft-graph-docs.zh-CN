# <a name="subscription-resource-type"></a>订阅资源类型
订阅允许客户端应用接收有关 Microsoft Graph 数据的通知。当前可订阅以下数据集：

1. 邮件、事件及 Outlook 联系人
1. 来自 Office 组的对话。
1. 来自 OneDrive 的驱动器根项 


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string"
}

```
## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|changeType|string|指示订阅资源中将引发通知的更改类型。支持的值是：`created`、`updated`、`deleted`。可以使用以逗号分隔的列表组合多个值。|
|notificationUrl|string|将接收通知的端点的 URL。该 URL 必须使用 HTTPS 协议。|
|资源|string|指定要被监视以进行更改的资源。不包含基本 URL（“https://graph.microsoft.com/v1.0/”）。|
|expirationDateTime|[dateTime](http://tools.ietf.org/html/rfc3339)|指定 webhook 订阅过期的日期和时间。时间使用 UTC 格式，也可以是从订阅创建（因订阅资源不同而异）开始的一段时间。请参阅下表，获取最大值。|
|clientState|string|指定服务为每个通知发送的 `clientState` 属性的值。最大长度为 128 个字符。通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。|
|id|string|订阅的唯一标识符。只读。|

## <a name="maximum-expiration-times-per-resource"></a>每个资源的最大过期时间
| 资源 | 最大过期时间 |
|:---------------------|:--------------------|
|邮件| 4230 分钟。|
|日历| 4230 分钟。|
|联系人| 4230 分钟。|
|群组对话| 4230 分钟。|
|驱动器根项| 86400 分钟|

## <a name="relationships"></a>关系
无


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建订阅](../api/subscription_post_subscriptions.md) | [订阅](subscription.md) |订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。|
|[更新订阅](../api/subscription_update.md) | [订阅](subscription.md) |通过更新其过期时间来续订订阅。|
|[获取订阅](../api/subscription_get.md) | [订阅](subscription.md) |读取 subscription 对象的属性和关系。|
|[删除订阅](../api/subscription_delete.md) | 无 |删除订阅对象。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
