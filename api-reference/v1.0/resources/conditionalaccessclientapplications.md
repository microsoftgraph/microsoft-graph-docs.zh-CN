---
title: conditionalAccessClientApplications 资源类型
description: 表示 (策略范围中包含和排除) 服务主体和工作负荷标识的客户端应用程序。
author: calebb
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0afcbcc68291d73aa83f9d730d81c257932c1dd7
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819060"
---
# <a name="conditionalaccessclientapplications-resource-type"></a>conditionalAccessClientApplications 资源类型

命名空间：microsoft.graph

表示 (策略范围中包含和排除) 服务主体和工作负荷标识的客户端应用程序。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|excludeServicePrincipals|String collection|从策略范围中排除的服务主体 ID。|
|includeServicePrincipals|String collection|策略范围中包含的服务主体 ID，或 `ServicePrincipalsInMyTenant`。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessClientApplications"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessClientApplications",
  "includeServicePrincipals": [
    "String"
  ],
  "excludeServicePrincipals": [
    "String"
  ]
}
```

