---
title: audioSourceLevel 资源类型
description: 其他源的级别配置。
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 35997bfcae7f33cc9bf8e62121c5dc2a724c95be
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913742"
---
# <a name="audiosourcelevel-resource-type"></a>audioSourceLevel 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

其他源的级别配置。

## <a name="properties"></a>属性

| 属性               | 类型    | 说明                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| duckOthers             | Boolean | 允许此源在活动时有其他源。 如果设置为 true，则必须设置 ducking 级别。|
| 块级                  | Int64   | 源的 Ducking 级别（如果`duckOthers`设置为`true`）。                                     |
| 参与者            | String  | 源参与者音频流。                                                                |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioSourceLevel"
}-->
```json
{
  "duckOthers": true,
  "level": 100,
  "participant": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
