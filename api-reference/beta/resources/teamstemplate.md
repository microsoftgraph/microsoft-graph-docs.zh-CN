---
title: teamsTemplate 资源类型
description: 描述 teamsTemplate 实体。
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d20d759476177541ed51ff40edec6188290cbbb1
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690019"
---
# <a name="teamstemplate-resource-type"></a>teamsTemplate 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

团队模板是用于在 Microsoft Teams 中创建 [团队](../resources/team.md) 的蓝图。 模板指定应在使用模板创建的新团队中预配的结构、设置甚至内容。 Microsoft 提供了一套基本模板，客户可以保存自己的自定义模板。

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

- [团队](team.md)
- [teamTemplateDefinition](teamtemplatedefinition.md)



