---
title: teamFunSettings 资源类型
description: 要配置的团队中的使用 Giphy、 memes 和标签的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: c701ffe76c82a6cb4b3586272926290f634a02d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987669"
---
# <a name="teamfunsettings-resource-type"></a>teamFunSettings 资源类型



要配置的设置使用 Giphy、 memes 和[团队](team.md)中的标签。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowGiphy|布尔|如果设置为 true，则启用 Giphy 使用。|
|giphyContentRating|字符串 (enum)|Giphy 内容评级。 可取值为：`moderate`、`strict`。|
|allowStickersAndMemes|布尔|如果设置为 true，使用户能够包括标签和 memes。|
|allowCustomMemes|布尔|如果设置为 true，使用户能够包括自定义 memes。|

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
