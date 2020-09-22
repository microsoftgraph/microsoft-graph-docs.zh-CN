---
title: mediaStream 资源类型
description: MediaStream 类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d1158dfb01b9e92c5dc97f34bef3bb3661da51b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088487"
---
# <a name="mediastream-resource-type"></a>mediaStream 资源类型

命名空间：microsoft.graph

其中包含媒体通道的相关信息。

## <a name="properties"></a>属性

| 属性    | 类型    | 说明                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | 方向。 可能的值为 `inactive` 、 `sendOnly` 、 `receiveOnly` 、 `sendReceive` 。                  |
| label       | String  | 媒体流标签。                                                                                       |
| mediaType   | String  | 媒体类型。 可能的值为 `unknown` 、、、 `audio` `video` `videoBasedScreenSharing` `data` 。        |
| serverMuted | Boolean | 如果服务器已将媒体设为静音。                                                                          |
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

