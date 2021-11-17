---
title: excludeTarget 资源类型
description: 表示从策略中排除的用户或用户组。
author: mjsantani
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 368d6446d9dbead0ccacfb5538c3433050b6c79c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034403"
---
# <a name="excludetarget-resource-type"></a>excludeTarget 资源类型

命名空间：microsoft.graph

表示从策略中排除的用户或用户组。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户或组Azure Active Directory标识符。|
|targetType|authenticationMethodTargetType|身份验证方法目标的类型。 可取值为：`user`、`group`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludeTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludeTarget",
  "id": "String (identifier)",
  "targetType": "String"
}
```
