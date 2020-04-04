---
title: 订阅资源类型
description: 借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8ede2274abebbba1148762f5d3606cd61a4578a4
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108429"
---
# <a name="subscription-resource-type"></a>订阅资源类型

命名空间：microsoft.graph

借助订阅，客户端应用可以接收有关 Microsoft Graph 数据更改的通知。 目前，支持订阅以下资源：

- Microsoft Graph 安全性 API 中的[警报][]
- Office 365 组的[对话][]
- OneDrive for Business 中根文件夹[driveItem][] 的层次结构中的内容，或用户个人 OneDrive 中的根文件夹或子文件夹 [driveItem][] 的层次结构中的内容
- SharePoint [网站][]下的[列表][] 
- Outlook 中的[邮件][]、[事件][]或[联系人][]
- Azure Active Directory 中的[用户][]或[组][]

查看“[使用 Microsoft Graph API 获取更改通知](webhooks.md)”了解各支持资源的可能资源路径值。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-------|:------------|:------------|
| [创建订阅](../api/subscription-post-subscriptions.md) | [订阅](subscription.md) | 订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。 |
| [更新订阅](../api/subscription-update.md) | [订阅](subscription.md) | 通过更新其过期时间来续订订阅。 |
| [列出订阅](../api/subscription-list.md) | [订阅](subscription.md) | 列出有效订阅。 |
| [获取订阅](../api/subscription-get.md) | [订阅](subscription.md) | 读取 subscription 对象的属性和关系。 |
| [删除订阅](../api/subscription-delete.md) | 无 | 删除订阅对象。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| changeType | string | 必需。 指示订阅资源中将引发通知的更改类型。 支持的值是：`created`、`updated`、`deleted`。 可以使用以逗号分隔的列表组合多个值。<br><br>注意：驱动器根项和列表通知仅支持 `updated` changeType。 用户和组通知支持 `updated` 和 `deleted` changeType。 |
| notificationUrl | string | 必需。 将接收通知的终结点的 URL。 该 URL 必须使用 HTTPS 协议。 |
| resource | string | 必需。 指定要被监视以进行更改的资源。 不包含的基 URL (`https://graph.microsoft.com/v1.0/`)。 查看各支持资源的可能资源路径[值](webhooks.md)。|
| expirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | 必需。 指定 webhook 订阅过期的日期和时间。 时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。  请参阅下表，了解支持的最长订阅有效期。 |
| clientState | 字符串 | 可选。 指定服务为每个通知发送的 `clientState` 属性的值。 最大长度为 128 个字符。 通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。 |
| id | string | 订阅的唯一标识符。只读。 |
| applicationId | string | 用于创建订阅的应用程序的标识符。 只读。 |
| creatorId | string | 已创建订阅的用户或服务主体的标识符。 如果此应用使用委派权限来创建订阅，则此字段包含该应用代表其调用的已登录用户的 ID。 如果此应用使用应用程序权限，则此字段包含对应于该应用的服务主体的 ID。 只读。 |
| latestSupportedTlsVersion | 字符串 | 指定由 **notificationUrl**指定的通知端点支持的 "传输层安全性 (TLS)" 的最新版本。 可能的值包括 `v1_0`、`v1_1`、`v1_2`、`v1_3`。 </br></br>对于通知终结点支持低于当前推荐版本（TLS 1.2）的版本的订阅者，通过设置 [Timeline](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) 指定此属性，可在完成升级到 TLS 1.2 前暂时使用其过时的 TLS 版本。 对于这些订阅者，不按时间线设置此属性会导致订阅操作失败。 </br></br>对于其通知端点已支持 TLS 1.2 的订阅者，设置此属性是可选的。 在这种情况下，Microsoft Graph 将属性默认设置为 `v1_2`。 |

### <a name="maximum-length-of-subscription-per-resource-type"></a>每个资源类型的最长订阅有效期

| Resource            | 最大过期时间  |
|:--------------------|:-------------------------|
| 用户、组和其他目录资源   | 4230 分钟（不到 3 天）    |
| 邮件                | 4230 分钟（不到 3 天）    |
| 日历            | 4230 分钟（不到 3 天）    |
| 联系人            | 4230 分钟（不到 3 天）    |
| 组对话 | 4230 分钟（不到 3 天）    |
| 驱动器根项    | 4230 分钟（不到 3 天）    |
| SharePoint 列表     | 4230 分钟（不到 3 天）    |
| 安全警报     | 43200分钟（不到 30 天）  |

> **注意：** 现有和新的应用都不得超过支持的这一上限值。 今后，任何超出最大值的订阅创建或续订请求都将失败。

## <a name="relationships"></a>关系

无

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
  "creatorId": "string",
  "latestSupportedTlsVersion": "string"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
