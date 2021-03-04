---
title: conditionalAccessDevices 资源类型
description: 表示策略作用域中的设备。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a42e6023ace493c5efb230ffd53eb9c4caee7d16
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440526"
---
# <a name="conditionalaccessdevices-resource-type"></a>conditionalAccessDevices 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示策略作用域中的设备。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| includeDevices | 字符串集合 | 策略范围内状态。 `All` 是唯一允许的值。 |
| excludeDevices | 字符串集合 | 策略作用域中排除的国家/省/市/ 可能的值： `Compliant` `DomainJoined` ， 。 |
| includeDeviceStates (弃) | 字符串集合 | 策略范围内状态。 `All` 是唯一允许的值。 |
| excludeDeviceStates (已弃) | 字符串集合 | 策略作用域中排除的国家/省/市/ 可能的值： `Compliant` `DomainJoined` ， 。 |

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


