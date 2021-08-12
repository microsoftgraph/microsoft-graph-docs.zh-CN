---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。
localization_priority: Normal
author: spunukol
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: c2bdac56da724cecce33a43a360ef4cbcdcae6ffea680a35169ce9052d71eeea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229388"
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

