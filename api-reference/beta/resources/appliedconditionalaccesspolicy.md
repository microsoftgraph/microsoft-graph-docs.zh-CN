---
title: appliedConditionalAccessPolicy 资源类型
description: 指示与由相应登录活动触发的已应用的条件访问策略相关的属性。
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c675d79598ff4428f3384518edc74cfcb8cc050d
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665856"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>appliedConditionalAccessPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示与由相应登录活动触发的已应用的条件访问策略相关的属性。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|conditionsSatisfied|conditionalAccessConditions|引用满足的条件访问策略条件。 可取值为：`none`、`application`、`users`、`devicePlatform`、`location`、`clientType`、`signInRisk`、`userRisk`、`time`、`deviceState`、`client`。|
|conditionsNotSatisfied|conditionalAccessConditions|引用不满足的条件访问策略条件。 可取值为：`none`、`application`、`users`、`devicePlatform`、`location`、`clientType`、`signInRisk`、`userRisk`、`time`、`deviceState`、`client`。|
|enforcedGrantControls|String 集合|请参阅条件访问策略强制实施的授予 (示例："需要多重身份验证") 。|
|enforcedSessionControls|String 集合|引用条件访问策略强制的会话 (示例："要求应用强制执行的控件") 。|
|id|String|条件访问策略的标识符。|
|result|appliedConditionalAccessPolicyResult| 指示触发的 CA 策略的结果。 可能的值是：、、 (Policy 未应用，因为策略条件未满足) ， (这是因为策略处于禁用状态 `success` `failure` `notApplied` `notEnabled` `unknown` `unknownFutureValue` `reportOnlySuccess` `reportOnlyFailure` `reportOnlyNotApplied` `reportOnlyInterrupted`) 、。 请注意，必须使用请求标头获取此可发展枚举中的以下值 `Prefer: include-unknown-enum-members` [](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `reportOnlySuccess` `reportOnlyFailure` ：、、、。 `reportOnlyNotApplied` `reportOnlyInterrupted`|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
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
  "description": "appliedConditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
