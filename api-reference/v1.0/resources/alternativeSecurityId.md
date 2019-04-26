---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。
localization_priority: Normal
ms.openlocfilehash: 23ef74085a4a3cc383f0854e9139c9a0b63e3d40
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569478"
---
# <a name="alternativesecurityid-resource-type"></a>alternativeSecurityId 资源类型

仅供内部使用。

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
