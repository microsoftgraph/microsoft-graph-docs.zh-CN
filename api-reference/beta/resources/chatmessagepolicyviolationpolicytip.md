---
title: chatMessagePolicyViolationPolicyTip 资源类型
description: 表示 chatMessagePolicyViolation 对象上策略提示的属性。 策略提示向发件人提供有关策略违反的信息。
author: RamjotSingh
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c315dbcb37b11e7ed5771544f511c5cf07cc89a8
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582247"
---
# <a name="chatmessagepolicytip-resource-type"></a>chatMessagePolicyTip 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [chatMessagePolicyViolation](chatmessagepolicyviolation.md) 对象上策略提示的属性。 策略提示向发件人提供有关策略违反的信息。
策略提示通常由 DLP (DLP) 设置，用于监视包含用户不应该发送的数据的邮件。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|complianceUrl|string|用户可以访问的 URL 来阅读有关组织的数据丢失防护策略的信息。  (，有关用户不应在聊天内容中说出内容) |
|generalText|string|向邮件发件人显示的解释性文本。|
|matchedConditionDescriptions|string 集合|邮件中由数据丢失防护应用检测到的不正确数据的列表。 每个 DLP 应用都定义自己的条件，例如"信用卡号"和"社会保险号"。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "generalText"
  ],
  "@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip"
}-->
```json
{
  "complianceUrl": "string",
  "generalText": "string",
  "matchedConditionDescriptions": ["string 1", "string 2"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "policy violation policy tip resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
