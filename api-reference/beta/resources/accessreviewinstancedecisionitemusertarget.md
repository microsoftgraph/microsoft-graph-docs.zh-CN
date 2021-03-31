---
title: accessReviewInstanceDecisionItemUserTarget 资源类型
description: 表示作为用户审阅的目标。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f10796937aa99e5808cb51bdb4069bd99d645db2
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "51469211"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a>accessReviewInstanceDecisionItemUserTarget 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示 [accessReviewInstance 中正在审阅的用户标识](accessreviewinstance.md)。

继承自 [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| userDisplayName | String | 用户的名称。 |
| userId | String | 用户的标识符。 |
| userPrincipalName | String | 用户主体名称。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemUserTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```
