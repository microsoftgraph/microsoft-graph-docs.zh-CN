---
title: 订阅资源类型
description: '订阅允许客户端应用在 Microsoft Graph 中接收有关数据更改的通知。 当前为以下资源启用了订阅:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9de48cc6a3e5dde459673117d9ee00a34477faf6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163936"
---
# <a name="subscription-resource-type"></a>订阅资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

订阅允许客户端应用在 Microsoft Graph 中接收有关数据更改的通知。 当前为以下资源启用了订阅:

- Outlook 中的[邮件][]、[事件][]或[联系人][]
- Office 365 组的[对话][]
- OneDrive for business 中根文件夹[driveItem][]的层次结构中的内容, 或用户个人 OneDrive 中的根文件夹或子文件夹[driveItem][]的内容
- Azure Active Directory 中的[用户][]或[组][]
- 来自 Microsoft Graph 安全性 API 的[警报][]


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
| changeType | string | 必需。 指示订阅资源中将引发通知的更改类型。 支持的值是：`created`、`updated`、`deleted`。 可以使用以逗号分隔的列表组合多个值。 <br><br>注意: 驱动器根项通知仅支持`updated` changeType。 用户和组通知支持`updated`和`deleted` changeType。 |
| notificationUrl | string | 必需。 将接收通知的终结点的 URL。 此 URL 必须使用 HTTPS 协议。 |
| resource | 字符串 | 必需。 指定将监视其更改的资源。 不包括基 URL (`https://graph.microsoft.com/beta/`)。 |
| expirationDateTime | DateTimeOffset | 必需。 指定 webhook 订阅过期的日期和时间。 时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。  请参阅下表，了解支持的最长订阅有效期。 |
| clientState | string | 可选。 指定服务为每个通知发送的 `clientState` 属性的值。 最大长度为 255 个字符。 通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。 |
| id | string | 订阅的唯一标识符。只读。 |
| applicationId | string | 用于创建订阅的应用程序的标识符。 只读。 |
| creatorId | string | 创建订阅的用户或服务主体的标识符。 如果应用程序使用委派权限来创建订阅, 则此字段包含代表已登录的用户的 id, 该应用代表。 如果应用程序使用的是应用程序权限, 则此字段包含与该应用对应的服务主体的 id。 只读。 |

## <a name="maximum-length-of-subscription-per-resource-type"></a>每个资源类型的最长订阅有效期

| 资源            | 最大过期时间  |
|:--------------------|:-------------------------|
| 邮件                | 4230分钟 (3 天内)    |
| 日历            | 4230分钟 (3 天内)    |
| 联系人            | 4230分钟 (3 天内)    |
| 组对话 | 4230分钟 (3 天内)    |
| 驱动器根项    | 4230分钟 (3 天内)    |
| 安全警报     | 43200分钟 (30 天内)  |

> **注意:** 现有应用程序和新应用程序不应超过支持的值。 将来, 创建或续订超出最大值的订阅的任何请求都将失败。

## <a name="relationships"></a>关系

无

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-------|:------------|:------------|
| [创建订阅](../api/subscription-post-subscriptions.md) | [订阅](subscription.md) | 订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。 |
| [更新订阅](../api/subscription-update.md) | [订阅](subscription.md) | 通过更新其过期时间来续订订阅。 |
| [列出订阅](../api/subscription-list.md) | [订阅](subscription.md) | 列出活动订阅。 |
| [获取订阅](../api/subscription-get.md) | [订阅](subscription.md) | 读取订阅对象的属性和关系。 |
| [删除订阅](../api/subscription-delete.md) | 无 | 删除订阅对象。 |

[contact]: ./contact.md
[对话]: ./conversation.md
[driveItem]: ./driveitem.md
[事件]: ./event.md
[group]: ./group.md
[message]: ./message.md
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
  "suppressions": [
    "Error: /api-reference/beta/resources/subscription.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
