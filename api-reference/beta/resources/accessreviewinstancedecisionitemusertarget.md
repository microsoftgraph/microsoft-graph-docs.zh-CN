---
title: accessReviewInstanceDecisionItemUserTarget 资源类型
description: 将评审的目标表示为用户。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aa2117895599ba1d2c4b9829b7cad22b581f2055
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000841"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a>accessReviewInstanceDecisionItemUserTarget 资源类型

命名空间：microsoft.graph

代表 [accessReviewInstance](accessreviewinstance.md)中的 "审阅" 下的用户标识。

继承自 [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| userDisplayName | String | 用户的名称。 |
| userId | 字符串 | User 的标识符。 |
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
