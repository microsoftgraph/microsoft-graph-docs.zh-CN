---
title: continuousAccessEvaluationPolicy 资源类型
description: CAE (连续访问) 有助于实时管理身份验证会话。 CAE 允许客户通过支持即时吊销事件来处理对资源的访问权限。
author: jerrysai
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f34fdacf75b991ff339f4b7cdd823290438e8fea
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962635"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a>continuousAccessEvaluationPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

CAE (持续访问) 实时管理身份验证会话。 CAE 允许客户通过支持即时吊销事件来处理对资源的访问权限。  有关详细信息，请参阅连续 [访问评估](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 continuousAccessEvaluationPolicy](../api/continuousaccessevaluationpolicy-get.md)|[continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md)|读取 [continuousAccessEvaluationPolicy 对象](../resources/continuousaccessevaluationpolicy.md) 的属性。|
|[更新 continuousAccessEvaluationPolicy](../api/continuousaccessevaluationpolicy-update.md)|[continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md)|更新 [continuousAccessEvaluationPolicy 对象](../resources/continuousaccessevaluationpolicy.md) 的属性。|
|
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|当用户的访问被删除或客户端 IP 地址更改时，连续访问评估将自动阻止对资源和应用程序的访问。 只读。|
|displayName|String| 该值始终为 `Continuous Access Evaluation` 。 只读。|
|groups|String collection|作用域中用于评估的组标识符的集合。 当集合为空时，所有组都位于范围内。|
|id|String|指定 [continuousAccessEvaluationPolicy 对象的](#continuousaccessevaluationpolicy-resource-type) 标识符。 只读。|
|isEnabled|Boolean| `true` 指示是否应该执行连续访问评估;否则 `false` 为 。 |
|users|String collection|评估范围内用户标识符的集合。 当集合为空时，所有用户都位于范围内。|

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
