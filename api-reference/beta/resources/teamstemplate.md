---
title: teamsTemplate 资源类型
description: 描述 teamsTemplate 实体。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5fc40b9c2a5789c5bcd7ab5794e41c715223eff3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046384"
---
# <a name="teamstemplate-resource-type"></a>teamsTemplate 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

团队模板是在 Microsoft 团队中创建 [团队](../resources/team.md) 的蓝图。 模板指定应在使用模板创建的新团队中设置的结构、设置和偶数内容。 Microsoft 提供了一套基本模板，并且客户可以保存自己的自定义模板。

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | String   | 模板的唯一标识符。 不能为 null。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a>另请参阅

- [team](team.md)



