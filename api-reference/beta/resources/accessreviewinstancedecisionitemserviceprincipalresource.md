---
title: accessReviewInstanceDecisionItemServicePrincipalResource 资源类型
description: 表示通过 accessReviewInstanceDecisionItem 对象表示其资源访问权限的服务主体。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ac8fe67110f28c852aa3e8c3047f59c4325444e4
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697144"
---
# <a name="accessreviewinstancedecisionitemserviceprincipalresource-resource-type"></a>accessReviewInstanceDecisionItemServicePrincipalResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示通过 [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 对象表示其资源访问权限的服务主体。 **accessReviewInstanceDecisionItemServicePrincipalResource** 是一种开放类型，允许传入其他属性。

继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| appId | String | 已向其授予访问权限的应用程序的全局唯一标识符。 |
| displayName | String | 资源的显示名称。 继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。|
| id | String | 决策项资源的标识符。 继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。 |
| type | String | 资源的类型。 类型将始终为 `ServicePrincipal`.  继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。 |


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessreviewinstancedecisionitemserviceprincipalresource",
  "baseType": "microsoft.graph.accessReviewInstanceDecisionItemResource",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessreviewinstancedecisionitemserviceprincipalresource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "appId": "String"
}
```
