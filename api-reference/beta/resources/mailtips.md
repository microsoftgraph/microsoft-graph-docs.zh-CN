---
title: 邮件提示资源类型
description: '有关提示性消息收件人，它们撰写邮件时向用户显示。 例如，-外出消息 '
localization_priority: Normal
ms.openlocfilehash: 62955594412b2d42a4d05b4b13858c4e511605df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860639"
---
# <a name="mailtips-resource-type"></a>邮件提示资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

有关提示性消息收件人，它们撰写邮件时向用户显示。 例如，作为自动回复邮件收件人-外出邮件。


## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | 如果已被收件人设置，邮件自动回复的提示。 |
| customMailTip | 字符串 | 可在收件人的邮箱中设置自定义邮件提示。 |
| deliveryRestricted| 布尔 | 收件人的邮箱是否受限制，例如，接受从预定义列表的发件人的邮件拒绝来自发件人的预定义列表的邮件，或接受来自仅经过身份验证发件人的邮件。 |
| emailAddress | [emailAddress](../resources/emailaddress.md) | 若要获取的邮件提示收件人的电子邮件地址。 |
| error | [mailTipsError](../resources/mailtipserror.md) | 在[getMailTips](../api/user-getmailtips.md)操作过程中出现错误。 |
| externalMemberCount | Int32 | 如果收件人是通讯组列表的外部成员的数目。 |
| isModerated |布尔  | 是否向收件人发送邮件需要审批。 例如，如果收件人是大型通讯组列表和审阅者已设置最多批准邮件发送到该通讯组列表，或如果发送给邮件收件人需要审批的收件人的经理。 |
| mailboxFull | 布尔 | 收件人邮箱完全状态。 |
| maxMessageSize | Int32 | 收件人的组织或邮箱已配置最大邮件大小。 |
| recipientScope | 字符串 | 收件人范围。 可取值为：`none`、`internal`、`external`、`externalPartner`、`externalNonParther`。 例如，管理员可以设置其他组织为其"合作伙伴"。 如果管理员希望某些邮件提示可对特定范围有用范围。 也很有用，告知人的邮件可能离开组织，以帮助其选择正确决定哪些措词、 语气和内容的发件人。|
| recipientSuggestions | [recipient](../resources/recipient.md) collection | 收件人建议基于以前上下文它们出现在相同的邮件。 |
| totalMemberCount | Int32 | 如果收件人是通讯组列表成员的数目。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
