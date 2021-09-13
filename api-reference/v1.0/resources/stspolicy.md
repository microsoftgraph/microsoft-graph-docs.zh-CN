---
title: stsPolicy 资源类型
description: 表示控制策略行为的策略类型的抽象Microsoft 标识平台类型。
ms.localizationpriority: medium
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 04ab6b06bbe099759802a57b6bbfdc337a233ef6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59122962"
---
# <a name="stspolicy-resource-type"></a>stsPolicy 资源类型

命名空间：microsoft.graph

表示控制策略行为的策略类型的抽象[Microsoft 标识平台类型。](/azure/active-directory/develop/)

继承自 [policyBase](policyBase.md)。

## <a name="methods"></a>方法

无

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 此策略的唯一标识符。 只读。 继承自 [policyBase](policyBase.md)。|
|说明|String| 此策略的说明。 继承自 [policyBase](policyBase.md)。|
|displayName|String| 此策略的显示名称。 继承自 [policyBase](policyBase.md)。|
|definition|String collection| 包含 JSON 字符串的字符串集合，用于定义策略的规则和设置。 定义的语法因派生的策略类型不同而不同。 必填。|
|isOrganizationDefault|Boolean|如果设置为 true，则激活此策略。 同一策略类型可以有很多策略，但只有一个策略可以激活为组织默认策略。 可选，默认值为 false。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stsPolicy",
  "baseType": "microsoft.graph.policyBase",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": ["String"],
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stsPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
