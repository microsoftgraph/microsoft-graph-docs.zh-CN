---
title: conditionalAccessClientApplications 资源类型
description: 表示客户端应用程序 (策略作用域中包含) 排除的服务主体和工作负荷标识。
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ad30e86d9c434641e197338613f5f58cf5d2a788
ms.sourcegitcommit: de9df4bf6313b49afba74b6e9ef819907669c662
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2022
ms.locfileid: "62239371"
---
# <a name="conditionalaccessclientapplications-resource-type"></a>conditionalAccessClientApplications 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示客户端应用程序 (策略作用域中包含) 排除的服务主体和工作负荷标识。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|excludeServicePrincipals|String 集合|从策略作用域中排除的服务主体 ID。|
|includeServicePrincipals|String 集合|策略作用域中包含的服务主体 ID 或 `ServicePrincipalsInMyTenant` 。 |

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

