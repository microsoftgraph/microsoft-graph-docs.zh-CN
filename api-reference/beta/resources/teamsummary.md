---
title: teamSummary 资源类型
description: 包含有关网站中Microsoft Teams的信息，包括所有者、成员和来宾的数量。
ms.localizationpriority: medium
author: akhilkohlimicrosoft
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 497ac22cf95c30b4510c08b04e591c7acaf8c449
ms.sourcegitcommit: 0fa7148e0b776663eaca3e79e72b85046d4b8b1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/15/2022
ms.locfileid: "63500979"
---
# <a name="teamsummary-resource-type"></a>teamSummary 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关团队在Microsoft Teams的信息，包括所有者、成员和来宾的数量。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|guestsCount|Int32|团队中的来宾数。|
|membersCount|Int32|团队中的成员数。|
|ownersCount|Int32|团队中的所有者计数。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamSummary"
}-->

```json
{
    "guestsCount": "Integer",
    "membersCount": "Integer",
    "ownersCount": "Integer",
}
```


