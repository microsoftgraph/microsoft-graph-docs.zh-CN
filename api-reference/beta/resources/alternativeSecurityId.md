---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。 未来将弃用此复杂类型。
localization_priority: Normal
ms.openlocfilehash: 31e5501c504b8813f8910a8b8b352a1fa0ce9478
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/20/2019
ms.locfileid: "35083940"
---
# <a name="alternativesecurityid-resource-type"></a>alternativeSecurityId 资源类型

仅供内部使用。 未来将弃用此复杂类型。

## <a name="json-representation"></a>JSON 表示形式

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "type": 12345,
  "identityProvider": "string",
  "key": {"@odata.type": "Edm.Binary"}
}
```

## <a name="properties"></a>属性
| 属性         | 类型       | 说明
|:-----------------|:-----------|:---------------------
| 类型             | Int32      | 仅供内部使用
| identityProvider | string     | 仅供内部使用
| 注册表项              | Edm | 仅供内部使用
