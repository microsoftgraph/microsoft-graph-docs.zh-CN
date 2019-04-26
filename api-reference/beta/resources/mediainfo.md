---
title: mediaInfo 资源类型
description: 在提示操作中使用的媒体信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4c6f8e4f4ceea184f9663c433672d0892ed92467
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342637"
---
# <a name="mediainfo-resource-type"></a>mediaInfo 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在提示操作中使用的媒体信息。

## <a name="properties"></a>属性
| 属性       | 类型    | 说明                      |
|:---------------|:--------|:---------------------------------|
| resourceId     | String  | 资源的唯一标识。 |
| url            | String  | 资源的路径。            |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
