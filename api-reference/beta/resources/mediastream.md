---
title: mediaStream 资源类型
description: mediaStream 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 69d8088ba161bdf4dbf0482fdab8ad757347126d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342616"
---
# <a name="mediastream-resource-type"></a>mediaStream 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

mediaStream 类型。

## <a name="properties"></a>属性

| 属性    | 类型    | 说明                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | 方向。 可能的值为`inactive`、 `sendOnly`、 `receiveOnly`、 `sendReceive`。                  |
| label       | String  | 媒体流标签。                                                                                       |
| 群组   | String  | 媒体类型。 可能的值为`unknown`、 `audio` `video` `videoBasedScreenSharing`、、 `data`。        |
| serverMuted | Boolean | 如果服务器已将媒体设为静音。                                                                          |
| sourceId    | String  | 源 ID。                                                                                                |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted"
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

## <a name="example"></a>示例

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "sendReceive",
  "label": "main-audio",
  "mediaType": "audio",
  "serverMuted": false,
  "sourceId": "1024"
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
