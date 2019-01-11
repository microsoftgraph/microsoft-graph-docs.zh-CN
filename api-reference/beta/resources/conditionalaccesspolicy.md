---
title: conditionalAccessPolicy 资源类型
description: 指示由相应的登录活动触发条件的访问策略相关的属性
localization_priority: Normal
ms.openlocfilehash: 7b043e739f84715fb02fbdbd25599e5cfccc284a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820641"
---
# <a name="conditionalaccesspolicy-resource-type"></a>conditionalAccessPolicy 资源类型
指示由相应的登录活动触发条件的访问策略相关的属性



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|字符串|指的条件的访问策略的名称 (示例:"需要 MFA 的销售队伍")。|
|enforcedGrantControls|String 集合|指的是此条件访问策略强制实施的授予控件 (示例:"需要多因素身份验证")。|
|enforcedSessionControls|String 集合|指的是此条件访问策略强制实施的会话控件 (示例:"需要应用程序强制实施控件")。|
|id|字符串|条件访问策略的唯一 GUID|
|结果|字符串| 指示触发的 CA 策略的结果。可能的值为：<br/> `success` <br/> `failure` <br/> `notApplied`由于策略条件不满足，不应用策略。 <br/> `notEnabled`-这是由于处于禁用状态策略。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
}-->

```json
{
  "displayName": "String",
  "enforcedGrantControls": ["String"],
  "enforcedSessionControls": ["String"],
  "id": "String",
  "result": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
