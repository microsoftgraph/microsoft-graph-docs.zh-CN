---
title: teamsTemplate 资源类型
description: 介绍 teamsTemplate 实体。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c32c8cfa770bd7633915e0e8f9b6d371458d4173
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873412"
---
# <a name="teamstemplate-resource-type"></a>teamsTemplate 资源类型

命名空间：microsoft.graph

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

