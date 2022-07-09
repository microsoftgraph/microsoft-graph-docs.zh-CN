---
title: accessReviewInstanceDecisionItemUserTarget 资源类型
description: 表示以用户身份进行评审的目标。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f64e29f3b1ef13471147be495dcd100e80742304
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698126"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a>accessReviewInstanceDecisionItemUserTarget 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示 [accessReviewInstance](accessreviewinstance.md) 中正在审查的用户标识。

继承自 [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| userDisplayName | String | 用户的名称。 |
| userId | String | 用户的标识符。 |
| userPrincipalName | 字符串 | 用户主体名称。 |

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
