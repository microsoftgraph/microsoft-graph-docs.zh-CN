---
title: accessReviewInstanceDecisionItemServicePrincipalTarget 资源类型
description: 表示作为服务主体目标的评审目标。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dafb1cde55fe510edcff89bd5497997d136a12a9
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698140"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a>accessReviewInstanceDecisionItemServicePrincipalTarget 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示 [accessReviewInstance](accessreviewinstance.md) 中正在审查的服务主体。

继承自 [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md)。

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| servicePrincipalID | String | 正在审查其访问权限的服务主体的标识符。 |
| servicePrincipalDisplayName | 字符串 | 正在审查其访问权限的服务主体的显示名称。 |
| appId | String | 要评审的服务主体实体的 appId。 |

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
