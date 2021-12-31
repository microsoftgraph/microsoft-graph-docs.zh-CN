---
title: authenticationStrength 资源类型
description: 条件访问策略中强制执行的自定义身份验证强度
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a316d3d6f575183fcb59647355545746838b0cdf
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647214"
---
# <a name="authenticationstrength-resource-type"></a>authenticationStrength 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在条件访问策略中强制执行的自定义身份验证强度。 

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|authenticationStrengthId|String|身份验证强度的标识符。|
|displayName|String|身份验证强度的名称。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationStrength"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationStrength",
  "authenticationStrengthId": "String",
  "displayName": "String"
}
```

