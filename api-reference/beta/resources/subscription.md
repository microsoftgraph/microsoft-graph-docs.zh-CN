---
title: 订阅资源类型
description: 订阅允许客户端应用接收有关 Microsoft Graph 数据更改的通知。目前，支持订阅以下资源：
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: b78a6ef57245603ae511d1c3b59237993c87f46e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443121"
---
# <a name="subscription-resource-type"></a>订阅资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的变更通知。 目前，为以下资源启用了订阅。 

> **注意** 标记为星号* (*) 仅在 beta 终结点中受支持。

- Microsoft Graph 安全性 API 中的[警报][]。
- Microsoft Teams 中的通话或会议后生成的 [callRecord][]。
- Microsoft Teams [](./channel.md)中的频道。*
- Microsoft Teams [](./chat.md)中的聊天。*
- 通过 Microsoft Teams 中的团队或频道发送的 [chatMessage][]。
- Microsoft 365 组中的[对话][]。
- 团队、频道或聊天中的[conversationMember](./conversationmember.md) Microsoft Teams。*
- OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容。
- [Azure Active Directory。][]
- SharePoint [site][]下的[list][]。
- Outlook 中的[邮件][]、[事件][]或[联系人][]。
- 用户[状态][]Microsoft Teams。*
- Microsoft Teams [](./team.md)团队。*
- [打印机][] (当打印机的打印作业进入”JobFetchable”状态时 - 准备好提取打印) 和通用打印中的 [printTaskDefinition][]。 有关详细信息，请参阅 [订阅云打印 API 中的更改通知](/graph/universal-print-webhook-notifications)。
- a [todoTask][] of a user in 微软待办.*
- 用户[Azure Active Directory。][]

查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-------|:------------|:------------|
| [创建订阅](../api/subscription-post-subscriptions.md) | [订阅](subscription.md) | 订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收变更通知。 |
| [更新订阅](../api/subscription-update.md) | [订阅](subscription.md) | 通过更新其过期时间续订订阅。 |
| [列出订阅](../api/subscription-list.md) | [订阅](subscription.md) | 列出有效订阅。 |
| [获取订阅](../api/subscription-get.md) | [订阅](subscription.md) | 读取 subscription 对象的属性和关系。 |
| [删除订阅](../api/subscription-delete.md) | 无 | 删除订阅对象。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 | 支持的资源 |
|:---------|:-----|:------------|:--------------|
| applicationId | string | 用于创建订阅的应用程序的标识符。 只读。 | 全部 |
| changeType | string | 指示订阅资源中将引发变更通知的更改类型。 支持的值是：`created`、`updated`、`deleted`。 可以使用以逗号分隔的列表组合多个值。 必需项。 <br><br>注意：驱动器根项和列表变更通知仅支持 `updated` changeType。 用户和组的变更通知支持 `updated` 和 `deleted` changeType。 | 全部 |
| clientState | string | 指定服务在每个更改通知中发送的 **clientState** 属性的值。 最大长度为 255 个字符。 通过比较与订阅一起发送的 **clientState** 属性的值与每个更改通知一起收到的 **clientState** 属性的值，客户端可以检查更改通知是否来自服务。 可选。 | 全部 |
| creatorId | string | 已创建订阅的用户或服务主体的标识符。 如果应用使用委派权限创建订阅，则此字段包含代表应用调用的登录用户的 ID。 如果应用程序使用应用程序权限，则此字段包含与应用程序对应的服务主体的 ID。 只读。 | 全部 |
| encryptionCertificate | string | 带有公钥的证书 的base64 编码表示形式，用于对更改通知中的资源数据进行加密。 可选。 **includeResourceData** 为 true 时是必需的。 | 全部 |
| encryptionCertificateId | string | 自定义应用提供的标识符，用于帮助识别解密资源数据所需的证书。 可选。 **includeResourceData** 为 true 时是必需的。 | 全部 |
| expirationDateTime | DateTimeOffset | 指定 webhook 订阅过期的日期和时间。 时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。  请参阅下表，了解支持的最长订阅有效期。 必需项。 | 全部 |
| id | string | 订阅的唯一标识符。只读。 | 全部 |
| includeResourceData | 布尔值 | 设置为 `true` 时，更改通知[包括资源数据](/graph/webhooks-with-resource-data)（例如聊天消息的内容）。 可选。 | 全部 |
| latestSupportedTlsVersion | string | 指定由 **notificationUrl** 指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。 可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。 </br></br>对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。 对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。 </br></br>对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。 在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。 | 全部 |
| lifecycleNotificationUrl | string | 接收生命周期通知（包括 `subscriptionRemoved` 和 `missed` 通知）的终结点的 URL。 该 URL 必须使用 HTTPS 协议。 可选。 <br><br>[阅读](/graph/webhooks-lifecycle)有关 Outlook 资源如何使用生命周期通知的详细信息。 | 全部 |
| notificationContentType | 字符串 | MS Graph 所需的内容类型为更改支持的资源类型变更通知。 默认内容类型为“application/json”内容类型。 | 全部 |
| notificationQueryOptions | 字符串 | 用于指定目标资源值的 OData 查询选项。 当资源达到与此处所提供的查询选项相匹配的状态时，客户端会收到通知。 有了订阅创建有效负载中的新属性以及所有现有属性后，每当资源达到 “notificationQueryOptions” 属性中提到的所需状态时，Webhook 就会发送通知，例如当打印作业完成时、当打印作业资源 `isFetchable` 属性值变为 true 时，等等。 | [通用打印服务](/graph/universal-print-webhook-notifications) |
| notificationUrl | string | 接收更改通知的终结点的 URL。 该 URL 必须使用 HTTPS 协议。 必需项。 | 全部 |
| resource | string | 指定要被监视以进行更改的资源。 不包含的基 URL (`https://graph.microsoft.com/beta/`)。 查看各支持资源的可能资源路径[值](webhooks.md)。 必需项。 | 全部 |

### <a name="maximum-length-of-subscription-per-resource-type"></a>每个资源类型的最长订阅有效期

| Resource            | 最大过期时间  |
|:--------------------|:-------------------------|
| 安全 **警报**     | 43200分钟（不到 30 天）  |
| Teams **callRecord**    | 4230 分钟（不到 3 天）  |
| Teams **频道**    | 60 分钟（1 小时）  |
| Teams **聊天** | 60 分钟（1 小时） |
| Teams **chatMessage**    | 60 分钟（1 小时）  |
| Teams **conversationMember**    | 60 分钟（1 小时）  |
| Teams **团队**    | 60 分钟（1 小时）  |
| 组 **对话** | 4230 分钟（不到 3 天）    |
| OneDrive **driveItem**    | 42300 分钟（不到 30 天）    |
| SharePoint **列表**    | 42300 分钟（不到 30 天）    |
| Outlook **邮件**、**事件**、**联系人**              | 4230 分钟（不到 3 天）    |
| **用户**、**组**、其他目录资源   | 4230 分钟（不到 29 天）    |
| **状态**        | 60 分钟（1 小时） |
| 打印 **打印机** | 4230 分钟（不到 3 天）    |
| 打印 **printTaskDefinition** | 4230 分钟（不到 3 天）    |
| **todoTask**              | 4230 分钟（不到 3 天）    |


> **注意：** 现有和新的应用都不得超过支持的这一上限值。 今后，任何超出最大值的订阅创建或续订请求都将失败。

## <a name="relationships"></a>关系

无。

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
  "lifecycleNotificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string",
  "includeResourceData": "boolean",
  "encryptionCertificate": "string",
  "encryptionCertificateId": "string",
  "latestSupportedTlsVersion": "string",
  "notificationContentType": "string",
  "notificationQueryOptions": "string"
}
```

[contact]: ./contact.md
[对话]: ./conversation.md
[driveItem]: ./driveitem.md
[list]: ./list.md
[site]: ./site.md
[事件]: ./event.md
[组]: ./group.md
[邮件]: ./message.md
[用户]: ./user.md
[警报]: ./alert.md
[chatMessage]: ./chatmessage.md
[callRecord]: ./callrecords-callrecord.md
[状态]: ./presence.md
[打印机]: ./printer.md
[printTaskDefinition]: ./printtaskdefinition.md
[todoTask]: ./todotask.md

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


