---
title: appliedConditionalAccessPolicy 资源类型
description: 指示与由相应登录活动触发的已应用的条件访问策略相关的属性。
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3aa114c23888ccc6852314e2274b8a89ca440344
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761526"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>appliedConditionalAccessPolicy 资源类型

命名空间：microsoft.graph

指示与由相应登录活动触发的已应用的条件访问策略相关的属性。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|displayName|字符串|请参阅条件访问策略的名称，例如 (Salesforce 需要 MFA") 。|
|enforcedGrantControls|字符串集合|请参阅条件访问策略强制实施的授予 (示例："需要多重身份验证") 。|
|enforcedSessionControls|字符串集合|引用条件访问策略强制的会话 (示例："要求应用强制执行的控件") 。|
|id|字符串|条件访问策略的唯一 GUID。|
|result|字符串| 指示触发的 CA 策略的结果。 可能的值是：<br/>`success`<br/>`failure`<br/>`notApplied` - 未应用策略，因为未满足策略条件。<br/>`notEnabled` - 这是因为策略处于禁用状态。|

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

