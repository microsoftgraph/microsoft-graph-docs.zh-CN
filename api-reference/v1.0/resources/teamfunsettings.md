---
title: teamFunSettings 资源类型
description: 用于配置团队中 Giphy、成员和贴纸使用情况的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 62e944143bc7dd6eac13c911b38872708777dd76dc6a812869d9e0b0655bc38d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129965"
---
# <a name="teamfunsettings-resource-type"></a>teamFunSettings 资源类型

命名空间：microsoft.graph



设置配置 Giphy、Meme 和贴纸在团队中的[使用](team.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowGiphy|Boolean|如果设置为 true，则启用 Giphy 使用。|
|giphyContentRating|字符串 (枚举) |Giphy 内容分级。 可取值为：`moderate`、`strict`。|
|allowStickersAndMemes|Boolean|如果设置为 true，则允许用户包括贴纸和 Meme。|
|allowCustomMemes|Boolean|如果设置为 true，则允许用户包括自定义 Meme。|

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

