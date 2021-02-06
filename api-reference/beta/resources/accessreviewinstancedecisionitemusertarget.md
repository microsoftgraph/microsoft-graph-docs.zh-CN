---
title: accessReviewInstanceDecisionItemUserTarget 资源类型
description: 表示作为用户审阅的目标。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 73fba5b7329a6dd13ddc455b9ba327467dde9016
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133467"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a>accessReviewInstanceDecisionItemUserTarget 资源类型

命名空间：microsoft.graph

表示 [accessReviewInstance 中正在审查的用户标识](accessreviewinstance.md)。

继承自 [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| userDisplayName | String | 用户名。 |
| userId | 字符串 | 用户的标识符。 |
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
