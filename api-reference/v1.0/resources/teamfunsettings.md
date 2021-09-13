---
title: teamFunSettings 资源类型
description: 用于配置团队中 Giphy、成员和贴纸使用情况的设置。
ms.localizationpriority: medium
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 169ecc9ff2e3dfc542a6d055b84234f7a3f98039
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134344"
---
# <a name="teamfunsettings-resource-type"></a>teamFunSettings 资源类型

命名空间：microsoft.graph



设置在团队中配置 Giphy、Meme 和贴纸[的使用](team.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowGiphy|布尔值|如果设置为 true，则启用 Giphy 使用。|
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

