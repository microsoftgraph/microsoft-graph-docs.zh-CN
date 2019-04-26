---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。
localization_priority: Normal
ms.openlocfilehash: 60e45c6d914c64f92b9f15f78fda22372a23e91f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345839"
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
