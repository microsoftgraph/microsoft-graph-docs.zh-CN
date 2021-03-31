---
title: accessReviewInstanceDecisionItemServicePrincipalTarget 资源类型
description: 表示作为服务主体目标的审阅目标。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7d8032282d7ddaf41779b73f707b0749e3c82dd0
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "51469221"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a>accessReviewInstanceDecisionItemServicePrincipalTarget 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示 [accessReviewInstance 中正在审阅的服务主体](accessreviewinstance.md)。

继承自 [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md)。

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| servicePrincipalID | String | 正在检查其访问权限的服务主体的标识符。 |
| servicePrincipalDisplayName | String | 要显示名称访问的服务主体的组。 |
| appId | String | 要检查的服务主体实体的 appId。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemServicePrincipalTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemServicePrincipalTarget",
  "servicePrincipalId": "String",
  "servicePrincipalDisplayName": "String",
  "appId": "String"
}
```
