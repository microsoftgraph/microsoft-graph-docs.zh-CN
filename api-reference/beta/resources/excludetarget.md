---
title: excludeTarget 资源类型
description: 表示从策略中排除的用户或用户组。
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9d2786a6107e524fe00430658542dea374cae275
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682884"
---
# <a name="excludetarget-resource-type"></a>excludeTarget 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示从策略中排除的用户或用户组。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Azure AD 用户或组的对象标识符。|
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
