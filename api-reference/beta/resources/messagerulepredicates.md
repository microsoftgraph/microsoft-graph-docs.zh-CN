---
title: messageRulePredicates 资源类型
description: 表示适用于某个规则的一组条件和例外情况。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e4afb1d0d12ffb49bbba8bd7c012ca36656085ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522657"
---
# <a name="messagerulepredicates-resource-type"></a>messageRulePredicates 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示适用于某个规则的一组条件和例外情况。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| bodyContains | String 集合 | 表示应该出现在传入邮件正文中的字符串，以便条件或例外情况适用。 |
| bodyOrSubjectContains | String 集合 | 表示应该出现在传入邮件正文或主题中的字符串，以便条件或例外情况适用。 |
| categories | String 集合 | 表示传入邮件应标记的类别，以便条件或例外情况适用。 |
| fromAddresses | [recipient](recipient.md) collection | 表示传入邮件的特定发件人电子邮件地址，以便条件或例外情况适用。 |
| hasAttachments | Boolean | 指示传入的邮件是否必须包含附件，以便条件或例外情况适用。 |
| headerContains | String 集合 | 表示出现在传入邮件头中的字符串，以便条件或例外情况适用。 |
| importance | importance | 传入邮件上标记的重要性，以便条件或例外情况适用：`low`、`normal`、`high`。 |
| isApprovalRequest | 布尔 | 指示传入的邮件是否必须为审批请求，以便条件或例外情况适用。 |
| isAutomaticForward | 布尔 | 指示传入的邮件是否必须自动转发，以便条件或例外情况适用。 |
| isAutomaticReply | 布尔 | 指示传入的邮件是否必须自动答复，以便条件或例外情况适用。 |
| isEncrypted | 布尔 | 指示传入的邮件是否必须加密，以便条件或例外情况适用。 |
| isMeetingRequest | 布尔 | 指示传入的邮件是否必须为会议请求，以便条件或例外情况适用。 |
| isMeetingResponse | 布尔 | 指示传入的邮件是否必须为会议响应，以便条件或例外情况适用。 |
| isNonDeliveryReport | 布尔 | 指示传入的邮件是否必须为未送达报告，以便条件或例外情况适用。 |
| isPermissionControlled | 布尔 | 指示传入的邮件是否必须受权限控制（受 RMS 保护），以便条件或例外情况适用。 |
| isReadReceipt | 布尔 | 指示传入的邮件是否必须为已读回执，以便条件或例外情况适用。 |
| isSigned | 布尔 | 指示传入的邮件是否必须有 S/MIME 签名，以便条件或例外情况适用。 |
| isVoicemail | 布尔 | 指示传入的邮件是否必须有语音邮件，以便条件或例外情况适用。 |
| messageActionFlag | messageActionFlag  | 表示出现在传入邮件上的 flag-for-action 值，以便条件或例外情况适用。 可能的值为： `any`、 `call`、 `doNotForward` `followUp` `fyi` `forward` `noResponseNecessary` `read` `reply`、、、、、、、、 `review` `replyToAll`。 |
| notSentToMe | 布尔 | 指示邮箱所有者是否不能是传入邮件的收件人，以便条件或异常情况适用。 |
| recipientContains | String 集合 | 表示出现在传入邮件的 **toRecipients** 或 **ccRecipients** 属性中的字符串，以便条件或例外情况适用。 |
| senderContains | String 集合 | 表示出现在传入邮件的 **from** 属性中的字符串，以便条件或例外情况适用。 |
| sensitivity | 敏感度 | 表示必须在传入邮件上标记的敏感度级别，以便条件或例外情况适用。 可能的值包括 `normal`、`personal`、`private`、`confidential`。 |
| sentCcMe | 布尔 | 指示邮箱所有者是否必须在传入邮件的 **ccRecipients** 属性中，以便条件或异常情况适用。 |
| sentOnlyToMe | 布尔 | 指示邮箱所有者是否必须是传入邮件的唯一收件人，以便条件或异常情况适用。 |
| sentToAddresses | [recipient](recipient.md) collection | 表示必须已向其发送传入邮件的电子邮件地址，以便条件或例外情况适用。 |
| sentToMe | 布尔 | 指示邮箱所有者是否必须在传入邮件的 **toRecipients** 属性中，以便条件或异常情况适用。 |
| sentToOrCcMe | Boolean | 指示邮箱所有者是否必须在传入邮件的 **toRecipients** 或 **ccRecipients** 属性中，以便条件或异常情况适用。 |
| subjectContains | String 集合 | 表示出现在传入邮件主题中的字符串，以便条件或例外情况适用。 |
| withinSizeRange | [sizeRange](sizerange.md) | 表示传入邮件必须介于其中的最小大小和最大大小（以千字节为单位），以便条件或例外情况适用。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRulePredicates"
}-->

```json
{
  "bodyContains": ["String"],
  "bodyOrSubjectContains": ["String"],
  "categories": ["String"],
  "fromAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": "Boolean",
  "headerContains": ["String"],
  "importance": "String",
  "isApprovalRequest": "Boolean",
  "isAutomaticForward": "Boolean",
  "isAutomaticReply": "Boolean",
  "isEncrypted": "Boolean",
  "isMeetingRequest": "Boolean",
  "isMeetingResponse": "Boolean",
  "isNonDeliveryReport": "Boolean",
  "isPermissionControlled": "Boolean",
  "isReadReceipt": "Boolean",
  "isSigned": "Boolean",
  "isVoicemail": "Boolean",
  "messageActionFlag": "String",
  "notSentToMe": "Boolean",
  "recipientContains": ["String"],
  "senderContains": ["String"],
  "sensitivity": "String",
  "sentCcMe": "Boolean",
  "sentOnlyToMe": "Boolean",
  "sentToAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "sentToMe": "Boolean",
  "sentToOrCcMe": "Boolean",
  "subjectContains": ["String"],
  "withinSizeRange": {"@odata.type": "microsoft.graph.sizeRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRulePredicates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
