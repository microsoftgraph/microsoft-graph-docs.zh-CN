---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 39ca29e8f2cbe9ad2c861fc83856fe83c2164675
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216845"
---
# <a name="subscription-resource-type"></a>订阅资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：

- Microsoft Graph 安全性 API 中的[警报][]
- 通过 Microsoft 团队中的团队或频道发送的[了 chatmessage][]
- Office 365 组中的[对话][]
- OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容
- Outlook 中的[消息][]、[事件][]或[联系人][]
- Azure Active Directory 中的[用户][]或[组][]

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-------|:------------|:------------|
| [创建订阅](../api/subscription-post-subscriptions.md) | [订阅](subscription.md) | 订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。 |
| [更新订阅](../api/subscription-update.md) | [订阅](subscription.md) | 通过更新其过期时间来续订订阅。 |
| [列出订阅](../api/subscription-list.md) | [订阅](subscription.md) | 列出有效订阅。 |
| [获取订阅](../api/subscription-get.md) | [订阅](subscription.md) | 读取订阅对象的属性和关系。 |
| [删除订阅](../api/subscription-delete.md) | 无 | 删除订阅对象。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| changeType | string | 指示订阅资源中将引发通知的更改类型。 支持的值是：`created`、`updated`、`deleted`。 可以使用以逗号分隔的列表组合多个值。 必需。 <br><br>注意：驱动器根项通知仅支持 `updated` changeType。 用户和组通知支持 `updated` 和 `deleted` changeType。 |
| notificationUrl | string | 接收通知的终结点的 URL。 该 URL 必须使用 HTTPS 协议。 必需。 |
| lifecycleNotificationUrl | string | 接收生命周期通知（包括`subscriptionRemoved`和`missed`通知）的终结点的 URL。 如果未提供，这些通知将传递给**notificationUrl**。 该 URL 必须使用 HTTPS 协议。 可选。 <br><br>[阅读](/graph/webhooks-outlook-authz)有关 Outlook 资源如何使用生命周期通知的详细信息。 |
| resource | string | 指定要被监视以进行更改的资源。 不包含的基 URL (`https://graph.microsoft.com/beta/`)。 必需。 |
| expirationDateTime | DateTimeOffset | 指定 webhook 订阅过期的日期和时间。 时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。  请参阅下表，了解支持的最长订阅有效期。 必需。 |
| clientState | string | 指定每个通知中由服务发送的**clientState**属性的值。 最大长度为 255 个字符。 客户端可以通过将随订阅发送的**clientState**属性的值与每个通知收到的**clientState**属性的值进行比较，来检查该通知是否来自服务。 可选。 |
| id | 字符串 | 订阅的唯一标识符。只读。 |
| applicationId | string | 用于创建订阅的应用程序的标识符。 只读。 |
| creatorId | string | 已创建订阅的用户或服务主体的标识符。 如果应用程序使用委派权限来创建订阅，则此字段包含代表已登录的用户的 ID，该应用代表。 如果应用程序使用的是应用程序权限，则此字段包含与该应用对应的服务主体的 ID。 只读。 |
| includeResourceData | Boolean | 当设置为`true`时，更改通知[包括资源数据](/graph/webhooks-with-resource-data)（如聊天邮件的内容）。 可选。 | 
| encryptionCertificate | string | 具有用于在通知中对资源数据进行加密的公钥的证书的 base64 编码表示形式。 可选。 当**includeResourceData**为 true 时是必需的。 | 
| encryptionCertificateId | string | 自定义应用程序提供的标识符，用于帮助确定解密资源数据所需的证书。 可选。 当**includeResourceData**为 true 时是必需的。 |

### <a name="maximum-length-of-subscription-per-resource-type"></a>每个资源类型的最长订阅有效期

| 资源            | 最长过期时间  |
|:--------------------|:-------------------------|
| 安全**警报**     | 43200分钟（不到 30 天）  |
| 团队**了 chatmessage**    | 60分钟（1小时）  |
| 组**对话** | 4230 分钟（不到 3 天）    |
| OneDrive **driveItem**    | 4230 分钟（不到 3 天）    |
| Outlook**邮件**、**事件**、**联系人**              | 4230 分钟（不到 3 天）    |
| **用户**、**组**、其他目录资源   | 4230 分钟（不到 3 天）    |


> **注意：** 现有和新的应用都不得超过支持的这一上限值。 今后，任何超出最大值的订阅创建或续订请求都将失败。

## <a name="relationships"></a>关系

无。

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
  "creatorId": "string",
  "includeResourceData": "boolean",
  "encryptionCertificate": "string",
  "encryptionCertificateId": "string"
}
```

[联系人]: ./contact.md
[对话]: ./conversation.md
[driveItem]: ./driveitem.md
[事件]: ./event.md
[组]: ./group.md
[邮件]: ./message.md
[用户]: ./user.md
[警报]: ./alert.md
[chatMessage]: ./chatmessage.md

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
