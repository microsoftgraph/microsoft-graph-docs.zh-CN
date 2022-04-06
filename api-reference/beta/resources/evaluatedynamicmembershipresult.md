---
title: evaluateDynamicMembershipResult 资源类型
description: 表示成员身份评估的结果。
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 551c2c87a09b7f2ddafc2079ab97c7f7e36837cd
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588517"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a>evaluateDynamicMembershipResult 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示成员身份评估的结果。

## <a name="properties"></a>属性

| 属性                        | 类型                                                          | 说明                                                                                                                                                                                                                                                                                                                                   |
| :------------------------------ | :------------------------------------------------------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| membershipRule                  | String                                                        | 如果提供了组 ID，则值为组的成员身份规则。 如果未提供组 ID，则值为作为参数提供的成员身份规则。 有关详细信息，请参阅 [Azure Active Directory 中的组动态成员资格规则](/azure/active-directory/users-groups-roles/groups-dynamic-membership)。 |
| membershipRuleEvaluationDetails | [expressionEvaluationDetails](expressionevaluationdetails.md) | 提供成员资格评估结果的详细分析。                                                                                                                                                                                                                                                                             |
| membershipRuleEvaluationResult  | Boolean                                                       | 如果用户 `true` 或设备是组的成员，则值为 。 如果提供了成员资格规则 `true` ，并且用户或设备通过规则评估，则值也可以为 ;否则为 `false`。                                                                                                                                      |

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
  "membershipRuleEvaluationDetails": {
    "@odata.type": "microsoft.graph.expressionEvaluationDetails"
  },
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
