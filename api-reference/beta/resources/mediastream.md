---
title: mediaStream 资源类型
description: 包含媒体通道的相关信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0274cdb1c35307e91e31c0b357ecf9a16e2d3f19
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913077"
---
# <a name="mediastream-resource-type"></a>mediaStream 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含媒体通道的相关信息。

## <a name="properties"></a>属性

| 属性    | 类型    | 说明                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | 方向。 可能的值为`inactive`、 `sendOnly`、 `receiveOnly`、 `sendReceive`。                  |
| label       | String  | 媒体流标签。                                                                                       |
| 群组   | String  | 媒体类型。 可能的值为`unknown`、 `audio` `video` `videoBasedScreenSharing`、、 `data`。        |
| serverMuted | Boolean | 指示服务器是否静音媒体。                                                                          |
| sourceId    | String  | 源 ID。                                                                                                |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted",
    "label"
  ],
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "inactive | sendOnly | receiveOnly | sendReceive",
  "label": "String",
  "mediaType": "unknown | audio | video | videoBasedScreenSharing | data",
  "serverMuted": true,
  "sourceId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
