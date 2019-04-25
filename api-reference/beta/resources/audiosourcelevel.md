---
title: audioSourceLevel 资源类型
description: 其他源的级别配置。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c91a4c57b283f7669b2be22bba5de5d958b437ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535576"
---
# <a name="audiosourcelevel-resource-type"></a>audioSourceLevel 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

其他源的级别配置。

## <a name="properties"></a>属性

| 属性               | 类型    | 说明                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| duckOthers             | 布尔值 | 允许此源在活动时有其他源。 如果设置为 true, 则必须设置 ducking 级别。|
| 块级                  | Int64   | 源的 Ducking 级别 (如果`duckOthers`设置为`true`)。                                     |
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
  "suppressions": [
    "Error: /api-reference/beta/resources/audiosourcelevel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
