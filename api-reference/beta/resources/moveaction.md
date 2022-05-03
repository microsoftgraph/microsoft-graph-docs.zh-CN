---
author: daspek
description: itemActivity 上存在 MoveAction 资源指示活动移动了一个项。
ms.date: 09/14/2017
title: MoveAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: f3622067f273a587174494d2ce3a68ed56540883
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176554"
---
# <a name="moveaction-resource-type"></a>MoveAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[**itemActivity**][activity] 上存在 **MoveAction** 资源指示活动移动了一个项。

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to&quot;: &quot;string"
}
```

## <a name="properties"></a>属性

| 属性 | 类型   | Description                                       |
| :------- | :----- | :------------------------------------------------ |
| from     | string | 被移动项原来位置的名称。 |
| to       | string | 将项移动到的位置的名称。   |

## <a name="remarks"></a>注解

项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": []
}
-->
