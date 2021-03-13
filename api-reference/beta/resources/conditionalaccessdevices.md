---
title: conditionalAccessDevices 资源类型
description: 表示策略作用域中的设备。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 94115e97c597bc34f03d843b8098f707ed39cd51
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761805"
---
# <a name="conditionalaccessdevices-resource-type"></a>conditionalAccessDevices 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示策略作用域中的设备。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| includeDevices | 字符串集合 | 策略作用域中的状态。 `All` 是唯一允许的值。 |
| excludeDevices | 字符串集合 | 策略作用域中排除的州。 可能的值 `Compliant` `DomainJoined` ：、。 |
| includeDeviceStates (弃) | 字符串集合 | 策略作用域中的状态。 `All` 是唯一允许的值。 |
| excludeDeviceStates (弃) | 字符串集合 | 策略作用域中排除的州。 可能的值 `Compliant` `DomainJoined` ：、。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeDevices",
    "excludeDevices"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "includeDevices": [ "String" ],
  "excludeDevices": [ "String" ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessDevices resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


