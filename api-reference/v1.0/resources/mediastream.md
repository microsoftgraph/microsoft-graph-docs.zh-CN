---
title: mediaStream 资源类型
description: mediaStream 类型。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4fa45c863bf06d2c1c2083a1f66796abcb46eaff
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134603"
---
# <a name="mediastream-resource-type"></a>mediaStream 资源类型

命名空间：microsoft.graph

这包含有关媒体通道的信息。

## <a name="properties"></a>属性

| 属性    | 类型    | 说明                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | 方向。 可能的值为 `inactive` `sendOnly` `receiveOnly` 、、、。 `sendReceive`                  |
| 标签       | String  | 媒体流标签。                                                                                       |
| mediaType   | String  | 媒体类型。 可能的值为 `unknown` `audio` `video` `videoBasedScreenSharing` `data` 、、。        |
| serverMuted | 布尔值 | 如果服务器将媒体设为静音。                                                                          |
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

