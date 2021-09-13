---
title: appliedConditionalAccessPolicy 资源类型
description: 指示与由相应登录活动触发的已应用的条件访问策略相关的属性。
ms.localizationpriority: medium
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 140402be929fc6d0d906b084251e21bab80f1a24
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078964"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>appliedConditionalAccessPolicy 资源类型

命名空间：microsoft.graph

指示与由相应登录活动触发的已应用的条件访问策略相关的属性。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|displayName|String|请参阅条件访问策略的名称，例如 (Salesforce 需要 MFA") 。|
|enforcedGrantControls|字符串集合|请参阅条件访问策略强制实施的授予 (示例："需要多重身份验证") 。|
|enforcedSessionControls|String collection|引用条件访问策略强制实施的会话 (示例："要求应用强制执行的控件") 。|
|id|String|条件访问策略的标识符。|
|result|appliedConditionalAccessPolicyResult| 指示触发的 CA 策略的结果。 可能的值包括：、、 (策略，因为策略条件未满足) ， (这是因为策略处于禁用状态 `success` `failure` `notApplied` `notEnabled`) 、 `unknown` `unknownFutureValue` 、 。|

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

