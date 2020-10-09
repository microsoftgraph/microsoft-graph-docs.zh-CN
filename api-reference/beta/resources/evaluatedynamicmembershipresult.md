---
title: evaluateDynamicMembershipResult 资源类型
description: 表示成员资格评估的结果。
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d00a2f1a0376c0d631354ea4f05c542dd4d1dcef
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402534"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a>evaluateDynamicMembershipResult 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示成员资格评估的结果。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| membershipRule | String | 如果提供了组 ID，则此值为组的成员身份规则。 如果未提供组 ID，则值是作为参数提供的成员身份规则。 有关详细信息，请参阅 [Azure Active Directory 中的组的动态成员身份规则](/azure/active-directory/users-groups-roles/groups-dynamic-membership)。 |
| membershipRuleEvaluationDetails | [expressionEvaluationDetails](expressionevaluationdetails.md) | 提供成员资格评估结果的详细 anaylsis。 |
| membershipRuleEvaluationResult | 布尔 | 值为 `true` 用户或设备是否为组的成员。 `true`如果提供了成员身份规则，并且用户或设备传递了规则评估，则也可以是值; 否则，也是如此 `false` 。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.evaluateDynamicMembershipResult",
  "baseType": null
}-->

```json
{
  "membershipRule": "String",
  "membershipRuleEvaluationDetails": {"@odata.type": "microsoft.graph.expressionEvaluationDetails"},
  "membershipRuleEvaluationResult": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "evaluateDynamicMembershipResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->