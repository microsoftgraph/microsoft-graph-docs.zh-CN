---
title: chatMessagePolicyViolation 资源类型
description: 表示聊天消息上的策略违反。 策略违反通常由 DLP 应用程序或 DLP (数据丢失) 设置。
author: RamjotSingh
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 46d839c6365c148777a280d7af8a36f3bf58ccd1
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582751"
---
# <a name="chatmessagepolicyviolation-resource-type"></a>chatMessagePolicyViolation 资源类型

表示聊天消息上的策略违反。 策略违反通常由 DLP 应用程序或 DLP (数据丢失) 设置。 DLP 应用程序监视包含用户不应该发送的数据的消息的聊天。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|dlpAction|**chatMessagePolicyViolationDlpActionType**|DLP 提供程序对包含敏感内容的邮件采取的操作。 支持的值为： <li>无</li><li>NotifySender -- 通知发件人违反，但允许读者阅读邮件。</li><li>BlockAccess -- 阻止读者阅读邮件。</li><li>BlockAccessExternal -- 阻止组织外部的用户阅读邮件，同时允许组织内部的用户阅读邮件。</li>|
|justificationText|string|替代策略违反时邮件发件人提供的理由文本。|
|policyTip|[chatMessagePolicyViolationPolicyTip](chatmessagepolicyviolationpolicytip.md)|要向邮件发件人显示有关邮件被标记为违反的原因的信息。 |
|userAction|**chatMessagePolicyViolationUserActionType**|指示用户对 DLP 提供程序阻止的邮件采取的操作。 支持的值为： <li>无</li><li>Override</li><li>ReportFalsePositive</li>当 DLP 提供程序更新邮件以阻止敏感内容时，不需要 userAction。|
|verdictDetails|**chatMessagePolicyViolationVerdictDetailsType**|指示发件人为响应策略违反可能采取的操作。 支持的值为： <li>无</li><li>AllowFalsePositiveOverride -- 允许发件人在 DLP 应用及其规则中声明策略Violation 为错误，并允许读者在 dlpAction 隐藏邮件时再次查看邮件。</li><li>AllowOverrideWithoutJustification -- 允许发件人过度处理 DLP 冲突，并允许读者在 dlpAction 隐藏邮件时再次查看邮件，而无需提供这样做的说明。 </li><li>AllowOverrideWithJustification -- 允许发件人过度处理 DLP 冲突，并允许读者在 dlpAction 隐藏邮件后再次查看邮件，并提供这样做的说明。</li>AllowOverrideWithoutJustification 和 AllowOverrideWithJustification 是互斥的。|

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
