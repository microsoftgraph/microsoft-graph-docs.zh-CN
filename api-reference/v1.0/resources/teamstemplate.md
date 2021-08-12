---
title: teamsTemplate 资源类型
description: 描述 teamsTemplate 实体。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5adcd554c687747fb45cdfd1a40e9e37cfaad2d9107a43ebc2ceca01b5d94f3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249123"
---
# <a name="teamstemplate-resource-type"></a>teamsTemplate 资源类型

命名空间：microsoft.graph

团队模板是创建新团队的[蓝图Microsoft Teams。](../resources/team.md) 模板指定应在使用该模板创建的新团队中设置的结构、设置甚至内容。 Microsoft 提供了一套基本模板，客户可以保存自己的自定义模板。

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


