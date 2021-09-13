---
title: teamsTemplate 资源类型
description: 描述 teamsTemplate 实体。
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3ef812716b2650e7919d18291f1f43c9adf878b5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098410"
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


