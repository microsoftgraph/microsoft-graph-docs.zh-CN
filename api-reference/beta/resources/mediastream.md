---
title: mediaStream 资源类型
description: MediaStream 类型。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 7e56448c2c6d284e7a5904f1b0af414166782907
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889612"
---
# <a name="mediastream-resource-type"></a>mediaStream 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

MediaStream 类型。

## <a name="properties"></a>属性

| 属性    | 类型    | Description                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| 方向   | 字符串  | 方向。 可能的值为`inactive`， `sendOnly`， `receiveOnly`， `sendReceive`。                  |
| 标签       | 字符串  | 媒体流标签。                                                                                       |
| 媒体类型   | 字符串  | 媒体类型。 可能的值是`unknown`， `audio`， `video`， `videoBasedScreenSharing`， `data`。        |
| serverMuted | 布尔 | 如果媒体服务器将设为静音。                                                                          |
| sourceId    | 字符串  | 源 id。                                                                                                |

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
<!-- {
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
