---
title: accessReviewInstanceDecisionItemServicePrincipalTarget 资源类型
description: 将评审的目标表示为服务主体目标。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e9943a287dd28a44f3b36eae1a92d1b2c385496c
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000842"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a>accessReviewInstanceDecisionItemServicePrincipalTarget 资源类型

命名空间：microsoft.graph

表示在 [accessReviewInstance](accessreviewinstance.md)中进行审阅的服务主体。

继承自 [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md)。

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| servicePrincipalID | 字符串 | 要查看其访问权限的服务主体的标识符。 |
| servicePrincipalDisplayName | 字符串 | 要查看其访问权限的服务主体的显示名称。 |
| appId | String | 要查看的服务主体实体的 appId。 |

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
