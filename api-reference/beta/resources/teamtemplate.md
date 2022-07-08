---
title: teamTemplate 资源类型
description: 表示同一团队模板的所有定义和版本的逻辑容器。
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 489818310abeb39ae4055c7360e8f1d909ea9525
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690120"
---
# <a name="teamtemplate-resource-type"></a>teamTemplate 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示同一团队模板的所有定义和版本的逻辑容器。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 teamTemplates](../api/teamwork-list-teamtemplates.md)|[teamTemplate](../resources/teamtemplatedefinition.md) 集合| 获取可用于租户的 **teamTemplate** 对象的列表。|
|[列表定义](../api/teamtemplate-list-definitions.md)| [teamTemplateDefinition](../resources/teamtemplatedefinition.md) 集合 | 列出与 **teamTemplate** 关联的 [teamTemplateDefinition](../resources/teamstemplate.md) 对象。  |

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | String   | 模板的唯一标识符。 不能为 null。 |

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|定义|[teamtemplatedefinition](../resources/teamtemplatedefinition.md) 集合| 具有特定结构和配置的团队的团队模板定义的通用表示形式。|

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamtemplate",
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a>另请参阅

- [团队](team.md)
- [teamTemplateDefinition](teamtemplatedefinition.md)
