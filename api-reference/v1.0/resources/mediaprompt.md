---
title: mediaPrompt 资源类型
description: 此资源类型包含有关要播放的音频文件和其他其他设置的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f981559ce5bac9bb597e49ff1b9d31e48413454b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871074"
---
# <a name="mediaprompt-resource-type"></a>mediaPrompt 资源类型

此资源类型包含有关要播放的音频文件和其他其他设置的信息。

## <a name="properties"></a>属性

| 属性    | 类型                      | 说明                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| mediaInfo   | [mediaInfo](mediainfo.md) | 媒体信息                                                           |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
