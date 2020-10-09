---
title: continuousAccessEvaluationPolicy 资源类型
description: 连续访问评估 (CAE) 有助于实时管理身份验证会话。 CAE 允许客户通过支持即时吊销事件来处理对资源的访问。
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8181c327a6ecc430d1bc631295dbc0482edb9eef
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404404"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a>continuousAccessEvaluationPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

连续访问评估 (CAE) 实时管理身份验证会话。 CAE 允许客户通过支持即时吊销事件来处理对资源的访问。  有关详细信息，请参阅 [连续访问评估](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 continuousAccessEvaluationPolicy](../api/continuousaccessevaluationpolicy-get.md)|[continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md)|读取 [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) 对象的属性。|
|[更新 continuousAccessEvaluationPolicy](../api/continuousaccessevaluationpolicy-update.md)|[continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md)|更新 [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) 对象的属性。|
|
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|字符串|连续访问评估会在用户的访问被删除或客户端 IP 地址更改时，自动阻止对资源和应用程序的即时访问。 只读。|
|displayName|字符串| 值始终为 "连续访问评估"。 只读。|
|groups|字符串集合|用于评估的范围内的组标识符的集合。 当集合为空时，所有组都在范围内。|
|id|字符串|指定 continuousAccessEvaluationPolicy 对象的标识符。 只读。|
|isEnabled|Boolean| `true` 以指示是否应执行连续访问评估;否则为 `false` 。 |
|users|字符串集合|评估范围内的用户标识符的集合。 当集合为空时，所有用户都在范围内。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "isEnabled": "Boolean",
  "users": [
    "String"
  ],
  "groups": [
    "String"
  ]
}
```