---
title: chatMessagePolicyViolationPolicyTip 资源类型
description: 表示 chatMessagePolicyViolation 对象上的策略提示的属性。 策略提示向发件人提供有关策略冲突的信息。
author: laujan
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1ccc3680f5b0365e1f54e9b82743b6906750b272
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223935"
---
# <a name="chatmessagepolicytip-resource-type"></a>chatMessagePolicyTip 资源类型

表示 [chatMessagePolicyViolation](chatmessagepolicyviolation.md) 对象上的策略提示的属性。 策略提示向发件人提供有关策略冲突的信息。
策略提示通常由数据丢失防护 (DLP) 应用程序设置，该应用程序监视包含用户不应发送的数据的邮件。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|complianceUrl|string|用户可访问的 URL，以了解有关组织的数据丢失防护策略的信息。  (ie，有关用户在聊天中不应说出的策略) |
|generalText|string|向邮件发件人显示的说明性文本。|
|matchedConditionDescriptions|string 集合|数据丢失防护应用程序检测到的消息中的不正确数据的列表。 每个 DLP 应用定义其自己的条件，例如 "信用卡号" 和 "社会保险号"。|

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
