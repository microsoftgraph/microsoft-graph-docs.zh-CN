---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 563d232d200797b87e894292e31eb48ad88bf540
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342877"
---
# <a name="subscription-resource-type"></a>订阅资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：

- Outlook 中的[消息][]、[事件][]或[联系人][]
- Office 365 组的[对话][]
- OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容
- Azure Active Directory 中的[用户][]或[组][]
- Microsoft Graph 安全性 API 中的[警报][]


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
  "lifecycleNotificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| changeType | string | 必需。 指示订阅资源中将引发通知的更改类型。 支持的值是：`created`、`updated`、`deleted`。 可以使用以逗号分隔的列表组合多个值。 <br><br>注意：驱动器根项通知仅支持 `updated` changeType。 用户和组通知支持 `updated` 和 `deleted` changeType。 |
| notificationUrl | string | 必需。 接收通知的终结点的 URL。 该 URL 必须使用 HTTPS 协议。 |
| lifecycleNotificationUrl | string | 可选。 接收生命周期通知 (包括`subscriptionRemoved`和`missed`通知) 的终结点的 URL。 如果未提供, 这些通知将传递给**notificationUrl**。 [阅读](/graph/webhooks-outlook-authz.md)有关 Outlook 资源如何使用生命周期通知的详细信息。  该 URL 必须使用 HTTPS 协议。 |
| resource | string | 必需。 指定要被监视以进行更改的资源。 不包含的基 URL (`https://graph.microsoft.com/beta/`)。 |
| expirationDateTime | DateTimeOffset | 必需。 指定 webhook 订阅过期的日期和时间。 时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。  请参阅下表，了解支持的最长订阅有效期。 |
| clientState | 字符串 | 可选。 指定服务为每个通知发送的 `clientState` 属性的值。 最大长度为 255 个字符。 通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。 |
| id | string | 订阅的唯一标识符。只读。 |
| applicationId | string | 用于创建订阅的应用程序的标识符。 只读。 |
| creatorId | string | 已创建订阅的用户或服务主体的标识符。 如果此应用使用委派权限来创建订阅，则此字段包含该应用代表其调用的已登录用户的 ID。 如果此应用使用应用程序权限，则此字段包含对应于该应用的服务主体的 ID。 只读。 |

## <a name="maximum-length-of-subscription-per-resource-type"></a>每个资源类型的最长订阅有效期

| 资源            | 最大过期时间  |
|:--------------------|:-------------------------|
| 邮件                | 4230 分钟（不到 3 天）    |
| 日历            | 4230 分钟（不到 3 天）    |
| 联系人            | 4230 分钟（不到 3 天）    |
| 组对话 | 4230 分钟（不到 3 天）    |
| 驱动器根项    | 4230 分钟（不到 3 天）    |
| 安全警报     | 43200分钟（不到 30 天）  |

> **注意：** 现有和新的应用都不得超过支持的这一上限值。 今后，任何超出最大值的订阅创建或续订请求都将失败。

## <a name="relationships"></a>关系

无

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-------|:------------|:------------|
| [创建订阅](../api/subscription-post-subscriptions.md) | [订阅](subscription.md) | 订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。 |
| [更新订阅](../api/subscription-update.md) | [订阅](subscription.md) | 通过更新其过期时间来续订订阅。 |
| [列出订阅](../api/subscription-list.md) | [订阅](subscription.md) | 列出有效订阅。 |
| [获取订阅](../api/subscription-get.md) | [订阅](subscription.md) | 读取订阅对象的属性和关系。 |
| [删除订阅](../api/subscription-delete.md) | 无 | 删除订阅对象。 |

[联系人]: ./contact.md
[对话]: ./conversation.md
[driveItem]: ./driveitem.md
[事件]: ./event.md
[组]: ./group.md
[邮件]: ./message.md
[用户]: ./user.md
[警报]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
