---
title: accessReviewInstanceDecisionItemAzureRoleResource 资源类型
description: 表示通过 accessReviewInstanceDecisionItem 对象表示其访问权限的 Azure 资源角色。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9b80801520e12b083e1a340a2e10caaf2b393f24
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162109"
---
# <a name="accessreviewinstancedecisionitemazureroleresource-resource-type"></a>accessReviewInstanceDecisionItemAzureRoleResource 资源类型

命名空间：microsoft.graph

表示通过 [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 对象表示其访问权限的 Azure 资源角色。 **accessReviewInstanceDecisionItemAzureRoleResource** 是允许传入其他属性的开放类型。

继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| displayName | String | Azure 角色的显示名称。 继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。|
| id | String | 决策项资源的标识符。 继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。 |
| type | String | 资源的类型。 类型将始终为 `AzureRole` 。  继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。 |
| 范围 | [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md) | 与此角色关联的作用域的详细信息。 |


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
