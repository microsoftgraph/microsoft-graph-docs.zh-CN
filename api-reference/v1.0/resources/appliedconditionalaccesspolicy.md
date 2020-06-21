---
title: appliedConditionalAccessPolicy 资源类型
description: 指示与应用的条件访问策略相关的属性，或与相应登录活动触发的策略相关的属性。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0e58058a174b630daa5022aed0dff78b7c2f3099
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788687"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>appliedConditionalAccessPolicy 资源类型

命名空间：microsoft.graph

指示与应用的条件访问策略相关的属性，或与相应登录活动触发的策略相关的属性。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|displayName|String|表示条件访问策略的名称（示例： "需要对 Salesforce 进行 MFA"）。|
|enforcedGrantControls|String collection|指由条件访问策略强制实施的授予控制（示例： "需要多重身份验证"）。|
|enforcedSessionControls|String collection|引用由条件访问策略强制实施的会话控件（示例： "需要应用强制性控制措施"）。|
|id|String|条件访问策略的唯一 GUID。|
|result|String| 指示已触发的 CA 策略的结果。 可能的值是：<br/>`success`<br/>`failure`<br/>`notApplied`-由于未满足策略条件，因此未应用策略。<br/>`notEnabled`-这是由于策略处于禁用状态。|

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
