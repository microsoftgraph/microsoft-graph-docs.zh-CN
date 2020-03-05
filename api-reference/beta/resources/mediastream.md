---
title: mediaStream 资源类型
description: 包含媒体通道的相关信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8d6bce42c31e39f5b36e3beccdac2fc660f9cb30
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522755"
---
# <a name="mediastream-resource-type"></a>mediaStream 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含媒体通道的相关信息。

## <a name="properties"></a>属性

| 属性    | 类型    | 说明                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | 方向。 可能的值为`inactive`、 `sendOnly`、 `receiveOnly`、 `sendReceive`。                  |
| label       | String  | 媒体流标签。                                                                                       |
| 群组   | String  | 媒体类型。 可能的值为`unknown`、 `audio` `video` `videoBasedScreenSharing`、、 `data`。        |
| serverMuted | 布尔 | 指示服务器是否静音媒体。                                                                          |
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
