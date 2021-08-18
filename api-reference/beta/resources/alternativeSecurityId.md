---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。 将来将弃用此复杂类型。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: spunukol
ms.openlocfilehash: 49d738554df8075a4ddec55c3b37d21c3c3d3ff7f18576f2d6deed92af583d53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249025"
---
# <a name="alternativesecurityid-resource-type"></a>alternativeSecurityId 资源类型

命名空间：microsoft.graph

仅供内部使用。 将来将弃用此复杂类型。

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
| 注册表项              | Edm.Binary | 仅供内部使用


