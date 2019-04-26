---
title: 邮件提示资源类型
description: '有关收件人的信息性消息, 在用户撰写邮件时向其显示。 例如, 外出邮件 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 15f026fd5a6485e5a0549d5987f53e26f0929b75
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342758"
---
# <a name="mailtips-resource-type"></a>邮件提示资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

有关收件人的信息性消息, 在用户撰写邮件时向其显示。 例如, 外出邮件作为邮件收件人的自动答复。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | "自动答复" 的邮件提示 (如果收件人已设置)。 |
| customMailTip | String | 可在收件人邮箱上设置的自定义邮件提示。 |
| deliveryRestricted| Boolean | 收件人邮箱是否受到限制, 例如, 仅接受来自预定义的发件人列表的邮件、拒绝来自预定义的发件人列表的邮件, 还是仅接受来自已验证的发件人的邮件。 |
| emailAddress | [emailAddress](../resources/emailaddress.md) | 要获取其邮件提示的收件人的电子邮件地址。 |
| error | [mailTipsError](../resources/mailtipserror.md) | [getMailTips](../api/user-getmailtips.md)操作过程中发生的错误。 |
| externalMemberCount | Int32 | 如果收件人是通讯组列表, 则为外部成员的数量。 |
| isModerated |Boolean  | 向收件人发送邮件是否需要审批。 例如, 如果收件人是一个大型通讯组列表, 并且已将仲裁人设置为审批发送到该通讯组列表的邮件, 或者向收件人发送邮件时需要对收件人的经理进行审批。 |
| mailboxFull | Boolean | 收件人的邮箱完整状态。 |
| maxMessageSize | Int32 | 已为收件人的组织或邮箱配置的最大邮件大小。 |
| recipientScope | String | 收件人的范围。 可取值为：`none`、`internal`、`external`、`externalPartner`、`externalNonParther`。 例如, 管理员可以将其他组织设置为其 "合作伙伴"。 如果管理员希望某些范围能够访问某些邮件提示, 则该范围很有用。 对于发件人来说, 通知他们其邮件可能会离开组织, 从而帮助他们做出正确的措辞、语气和内容决策。|
| recipientSuggestions | [recipient](../resources/recipient.md) collection | 根据以前的上下文显示在同一邮件中建议的收件人。 |
| totalMemberCount | Int32 | 如果收件人是通讯组列表, 则为成员数量。 |

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
