---
title: conditionalAccessDevices 资源类型
description: 表示策略作用域中的设备。
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0c4bc7721566bd8210830e51dbe820b1b44813e1
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996365"
---
# <a name="conditionalaccessdevices-resource-type"></a>conditionalAccessDevices 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示策略作用域中的设备。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| includeDevices | String collection | 策略作用域中的状态。 `All` 是唯一允许的值。 如果设置了 *deviceFIlter，则不能* 设置。 |
| excludeDevices | 字符串集合 | 策略作用域中排除的州。 可能的值 `Compliant` `DomainJoined` ：、。 如果设置了 **deviceFIlter，则不能** 设置。 |
| deviceFilter | [conditionalAccessFilter](conditionalaccessfilter.md) | 定义要包含/排除设备的动态设备语法规则的筛选器。 筛选器可以使用设备属性 (例如扩展属性) /排除它们。 如果设置了 **includeDevices** 或 **excludeDevices，则不能** 设置。 |
| includeDeviceStates (弃用) | 字符串集合 | 策略作用域中的状态。 `All` 是唯一允许的值。 |
| excludeDeviceStates (已弃) | 字符串集合 | 策略作用域中排除的州。 可能的值 `Compliant` `DomainJoined` ：、。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeDevices",
    "excludeDevices",
    "deviceFilter"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "includeDevices": [ "String" ],
  "excludeDevices": [ "String" ],
  "deviceFilter": {"@odata.type": "microsoft.graph.conditionalAccessFilter"}
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


