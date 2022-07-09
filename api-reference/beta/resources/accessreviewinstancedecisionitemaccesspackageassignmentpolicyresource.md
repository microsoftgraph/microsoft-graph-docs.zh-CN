---
title: accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource 资源类型
description: 表示通过 accessReviewInstanceDecisionItem 对象表示访问权限的访问包分配策略。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4ede4c067532e1925b5910bbfbb454e0db2a6b98
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697181"
---
# <a name="accessreviewinstancedecisionitemaccesspackageassignmentpolicyresource-resource-type"></a>accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示通过 [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 对象表示访问权限的访问包分配策略。 **accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource** 是允许传入其他属性的开放类型。

继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accessPackageDisplayName|String| 向其授予访问权限的访问包的显示名称。 |
|accessPackageId|String| 已向其授予访问权限的访问包的标识符。 |
| displayName | String | 访问包的显示名称。 继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。|
| id | 字符串 | 决策项资源的标识符。 继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。 |
| type | 字符串 | 资源的类型。 类型将始终为 `AccessPackageAssignmentPolicy`.  继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。 |



## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource",
  "baseType": "microsoft.graph.accessReviewInstanceDecisionItemResource",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "accessPackageId": "String",
  "accessPackageDisplayName": "String"
}
```
