---
title: mediaInfo 资源类型
description: 在提示操作中使用的媒体信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ef58bb2ca80ec18a1d11c0e3d2e976e6d7fa2bb9
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006667"
---
# <a name="mediainfo-resource-type"></a>mediaInfo 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在提示操作中使用的媒体信息。

## <a name="properties"></a>属性
| 属性       | 类型    | 说明                      |
|:---------------|:--------|:---------------------------------|
| resourceId     | String  | 可选，用于唯一标识资源。 如果传递了提示 uri，则会将此 resourceId 作为密钥进行缓存。 |
| url            | String  | 要播放的提示的路径。 目前仅支持带有16000（16KHz）采样速率的波形文件（.wav）格式的单通道、16位样本。 |


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
