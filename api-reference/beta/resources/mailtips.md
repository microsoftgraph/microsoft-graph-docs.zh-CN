---
title: 邮件提示资源类型
description: '有关收件人的信息性消息，在用户撰写邮件时向用户显示。 例如，外出邮件 '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0be2ee10807dadd4c8bd32dcec438f001fe8d481
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960416"
---
# <a name="mailtips-resource-type"></a>邮件提示资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

有关收件人的信息性消息，在用户撰写邮件时向用户显示。 例如，外出邮件作为邮件收件人的自动答复。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | 自动答复的邮件提示（如果收件人已设置）。 |
| customMailTip | String | 可以在收件人邮箱上设置的自定义邮件提示。 |
| deliveryRestricted| Boolean | 例如，是否限制收件人的邮箱，例如仅接受来自预定义发件人列表的邮件、拒绝来自预定义发件人列表的邮件或仅接受来自经过身份验证的发件人的邮件。 |
| emailAddress | [emailAddress](../resources/emailaddress.md) | 要获取其邮件提示的收件人的电子邮件地址。 |
| error | [mailTipsError](../resources/mailtipserror.md) | [getMailTips 操作期间发生的](../api/user-getmailtips.md)错误。 |
| externalMemberCount | Int32 | 如果收件人是通讯组列表，则外部成员的数量。 |
| isModerated |Boolean  | 是否向收件人发送邮件需要审批。 例如，如果收件人是一个大型通讯组列表，并且已设置仲裁人来批准发送到该通讯组列表的邮件，或者向收件人发送邮件需要收件人的经理批准。 |
| mailboxFull | Boolean | 收件人的邮箱完整状态。 |
| maxMessageSize | Int32 | 为收件人的组织或邮箱配置的最大邮件大小。 |
| recipientScope | recipientScopeType | 收件人的作用域。 可取值为：`none`、`internal`、`external`、`externalPartner`、`externalNonParther`。 例如，管理员可以将另一个组织设置为其"合作伙伴"。 如果管理员希望某些邮件提示可供某些作用域访问，则范围非常有用。 发件人还可以通知他们其邮件可能离开组织，帮助他们做出有关语气、语气和内容的正确决策。|
| recipientSuggestions | [recipient](../resources/recipient.md) collection | 基于之前在同一邮件中的显示上下文建议的收件人。 |
| totalMemberCount | Int32 | 如果收件人是通讯组列表，则成员数。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


