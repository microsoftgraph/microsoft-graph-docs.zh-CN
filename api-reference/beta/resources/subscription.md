---
title: Subscription 资源类型
description: 订阅允许的客户端应用程序以接收在 Microsoft Graph 中的数据的更改的通知。 目前，订阅启用以下资源：
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 265ea807330f833edf0d7b1f6a640e0a1f6f4634
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517265"
---
# <a name="subscription-resource-type"></a>订阅资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

订阅允许的客户端应用程序以接收在 Microsoft Graph 中的数据的更改的通知。 目前，订阅启用以下资源：

- Outlook 中的邮件、活动和联系人
- 来自 Office 组的对话。
- 来自 OneDrive 的驱动器根项
- 用户和 Azure Active Directory 组。
- 来自 Microsoft Graph 安全 API 的通知。

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
| changeType | string | 必需。 指示订阅资源中将引发通知的更改类型。 支持的值是：`created`、`updated`、`deleted`。 可以使用以逗号分隔的列表组合多个值。 <br><br>注意： 驱动器根项目通知仅支持`updated`changeType。 用户和组通知支持`updated`和`deleted`changeType。 |
| notificationUrl | string | 必需。 将接收通知的终结点 URL。 此 URL 必须进行使用 HTTPS 协议。 |
| 资源 | 字符串 | 必需。 指定将监视的更改的资源。 不包含的基 URL (`https://graph.microsoft.com/beta/`)。 |
| expirationDateTime | DateTimeOffset | 必需。 指定 webhook 订阅过期的日期和时间。 时间为 UTC 时间，可以是距离订阅创建的一段时间（因订阅资源不同而异）。  请参阅下表，了解支持的最长订阅有效期。 |
| clientState | string | 可选。 指定服务为每个通知发送的 `clientState` 属性的值。 最大长度为 255 个字符。 通过对比与订阅一起发送的 `clientState` 属性值和与每个通知一起接收的 `clientState` 属性值，客户端可以检查通知是否是由服务发送。 |
| id | string | 订阅的唯一标识符。只读。 |
| applicationId | string | 用于创建订阅的应用程序的标识符。 只读。 |
| creatorId | string | 用户或创建订阅的服务主体的标识符。 如果应用程序使用委派权限创建订阅，此字段包含应用程序调用代表登录用户的 id。 如果应用程序使用应用程序权限，此字段包含对应于应用程序的服务主体的 id。 只读。 |

## <a name="maximum-length-of-subscription-per-resource-type"></a>每个资源类型的最长订阅有效期

| 资源            | 最大过期时间  |
|:--------------------|:-------------------------|
| 邮件                | 4230 分钟 （在 3 天）    |
| 日历            | 4230 分钟 （在 3 天）    |
| 联系人            | 4230 分钟 （在 3 天）    |
| 组对话 | 4230 分钟 （在 3 天）    |
| 驱动器根项    | 4230 分钟 （在 3 天）    |
| 安全警报     | 43200 分钟 （在 30 天）  |

> **注意：** 现有应用程序和新的应用程序不应超过受支持的值。 将来，任何创建或更新的最大值超出订阅已请求将失败。

## <a name="relationships"></a>关系

无

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-------|:------------|:------------|
| [创建订阅](../api/subscription-post-subscriptions.md) | [订阅](subscription.md) | 订阅侦听器应用程序，在 Microsoft Graph 数据发生更改时接收通知。 |
| [更新订阅](../api/subscription-update.md) | [订阅](subscription.md) | 通过更新其过期时间续订。 |
| [列表订阅](../api/subscription-list.md) | [订阅](subscription.md) | 列出了活动订阅。 |
| [获取订阅](../api/subscription-get.md) | [订阅](subscription.md) | 读取属性和订阅对象的关系。 |
| [删除订阅](../api/subscription-delete.md) | 无 | 删除订阅对象。 |

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
