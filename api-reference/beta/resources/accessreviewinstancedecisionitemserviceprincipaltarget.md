---
title: accessReviewInstanceDecisionItemServicePrincipalTarget 资源类型
description: 表示作为服务主体目标的审阅目标。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ef944fdd1b8dbe989b1ad92e3d49b1b057fdef74
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133495"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a>accessReviewInstanceDecisionItemServicePrincipalTarget 资源类型

命名空间：microsoft.graph

表示 [accessReviewInstance 中正在审查的服务主体](accessreviewinstance.md)。

继承自 [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md)。

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| servicePrincipalID | 字符串 | 正在检查其访问权限的服务主体的标识符。 |
| servicePrincipalDisplayName | 字符串 | 正在显示名称其访问权限的服务主体的组。 |
| appId | String | 正在审查的服务主体实体的 appId。 |

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
