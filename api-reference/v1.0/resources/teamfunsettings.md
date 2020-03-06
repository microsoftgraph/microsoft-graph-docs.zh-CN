---
title: teamFunSettings 资源类型
description: 用于配置团队中 Giphy、成员和贴纸使用情况的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 696a6a3b02f90abe1456f99d9a40a4d9127b5697
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533548"
---
# <a name="teamfunsettings-resource-type"></a>teamFunSettings 资源类型

命名空间：microsoft.graph



用于配置在[团队](team.md)中使用 Giphy、meme 和不干胶标签的设置。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowGiphy|Boolean|如果设置为 true，将启用 Giphy。|
|giphyContentRating|String （enum）|Giphy 内容评级。 可取值为：`moderate`、`strict`。|
|allowStickersAndMemes|Boolean|如果设置为 true，则允许用户包括不干胶标签和 meme。|
|allowCustomMemes|Boolean|如果设置为 true，则允许用户包含自定义 meme。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
