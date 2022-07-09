---
title: accessReviewInstanceDecisionItemAzureRoleResource 资源类型
description: 表示通过 accessReviewInstanceDecisionItem 对象表示访问权限的 Azure 资源角色。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d607463664ee5c106e373a7bb568bfd32cd3c0a0
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697880"
---
# <a name="accessreviewinstancedecisionitemazureroleresource-resource-type"></a>accessReviewInstanceDecisionItemAzureRoleResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示通过 [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 对象表示访问权限的 Azure 资源角色。 **accessReviewInstanceDecisionItemAzureRoleResource** 是一种开放类型，允许传入其他属性。

继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| displayName | 字符串 | 显示 Azure 角色的名称。 继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。|
| id | String | 决策项资源的标识符。 继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。 |
| type | String | 资源的类型。 类型将始终为 `AzureRole`.  继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。 |
| 范围 | [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md) | 此角色关联的范围的详细信息。 |


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",
  "baseType": "microsoft.graph.accessReviewInstanceDecisionItemResource",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "scope": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
  }
}
```
