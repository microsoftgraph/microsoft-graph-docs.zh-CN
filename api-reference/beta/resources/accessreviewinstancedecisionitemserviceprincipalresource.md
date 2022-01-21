---
title: accessReviewInstanceDecisionItemServicePrincipalResource 资源类型
description: 表示通过 accessReviewInstanceDecisionItem 对象表示其资源访问权限的服务主体。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0ef1fa74401cc9c21f8e568ff988c037685d6f53
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161661"
---
# <a name="accessreviewinstancedecisionitemserviceprincipalresource-resource-type"></a>accessReviewInstanceDecisionItemServicePrincipalResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示通过 [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 对象表示其资源访问权限的服务主体。 **accessReviewInstanceDecisionItemServicePrincipalResource** 是允许传入其他属性的开放类型。

继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| appId | String | 已授予访问权限的应用程序的全局唯一标识符。 |
| displayName | String | 资源的显示名称。 继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。|
| id | String | 决策项资源的标识符。 继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。 |
| type | String | 资源的类型。 类型将始终为 `ServicePrincipal` 。  继承自 [accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md)。 |


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
