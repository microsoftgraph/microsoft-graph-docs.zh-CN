---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。 将来将弃用此复杂类型。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: spunukol
ms.openlocfilehash: 3e696c824e2229ea26cacccee11c93a24d03fa97
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547553"
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


