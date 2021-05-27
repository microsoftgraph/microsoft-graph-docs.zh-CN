---
title: evaluateDynamicMembershipResult 资源类型
description: 表示成员身份评估的结果。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 52621ee317183a59da418ecd35309cacc0637ae3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682640"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a>evaluateDynamicMembershipResult 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示成员身份评估的结果。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| membershipRule | String | 如果提供了组 ID，则值为组的成员身份规则。 如果未提供组 ID，则值为作为参数提供的成员身份规则。 有关详细信息，请参阅 Dynamic [membership rules for groups in Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership)。 |
| membershipRuleEvaluationDetails | [expressionEvaluationDetails](expressionevaluationdetails.md) | 提供成员资格评估结果的详细分析。 |
| membershipRuleEvaluationResult | Boolean | 如果 `true` 用户或设备是组的成员，则值为 。 如果提供了成员资格规则，并且用户或设备通过规则评估，则值也可以为 ; `true` 否则 `false` 为 。 |

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