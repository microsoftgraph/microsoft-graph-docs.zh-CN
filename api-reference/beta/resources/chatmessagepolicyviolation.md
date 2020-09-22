---
title: chatMessagePolicyViolation 资源类型
description: 代表聊天消息上的策略违规。 策略冲突通常由数据丢失防护 (DLP) 应用程序设置。
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 458e6440806ac57248bb87c6313d78b4845d647f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081984"
---
# <a name="chatmessagepolicyviolation-resource-type"></a>chatMessagePolicyViolation 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表聊天消息上的策略违规。 策略冲突通常由数据丢失防护 (DLP) 应用程序设置。 DLP 应用程序监视包含用户不应发送的数据的邮件的聊天。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|dlpAction|**chatMessagePolicyViolationDlpActionType**|DLP 提供程序对包含敏感内容的邮件执行的操作。 支持的值为： <li>无</li><li>NotifySender--将冲突的发件人通知给发件人，但允许读者阅读邮件。</li><li>BlockAccess--阻止读者阅读邮件。</li><li>BlockAccessExternal--阻止组织外部的用户阅读邮件，同时允许组织内的用户阅读邮件。</li>|
|justificationText|string|覆盖策略违规时邮件发件人提供的两端对齐文本。|
|policyTip|[chatMessagePolicyViolationPolicyTip](chatmessagepolicyviolationpolicytip.md)|向邮件发件人显示邮件被标记为冲突的原因的信息。 |
|userAction|**chatMessagePolicyViolationUserActionType**|指示用户对 DLP 提供程序阻止的邮件执行的操作。 支持的值为： <li>无</li><li>Override</li><li>ReportFalsePositive</li>当 DLP 提供程序更新邮件以阻止敏感内容时，userAction 不是必需的。|
|verdictDetails|**chatMessagePolicyViolationVerdictDetailsType**|指示发件人在响应策略冲突时可能采取的操作。 支持的值为： <li>无</li><li>AllowFalsePositiveOverride--允许发件人将 policyViolation 声明为 DLP 应用及其规则中的错误，并允许读者在 dlpAction 隐藏邮件时再次查看邮件。</li><li>AllowOverrideWithoutJustification--允许发件人 overriide DLP 违规，并允许读者在 dlpAction 隐藏邮件时再次查看邮件，而无需提供有关此操作的说明。 </li><li>AllowOverrideWithJustification--允许发件人 overriide DLP 违规，并允许读者在提供这样做的说明之后再次查看该邮件（如果 dlpAction 已隐藏）。</li>AllowOverrideWithoutJustification 和 AllowOverrideWithJustification 是相互排斥的。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userAction",
    "justificationText"
  ],
  "@odata.type": "microsoft.graph.chatMessagePolicyViolation"
}-->

```json
{
  "dlpAction": "string",
  "justificationText": "string",
  "policyTip": {"@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip"},
  "userAction": "string",
  "verdictDetails": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message policy violation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
