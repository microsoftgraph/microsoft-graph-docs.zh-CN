---
title: mediaInfo 资源类型
description: 提示操作中使用的媒体信息。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 40bde8c230843156d51b90db64a7e210686886f4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108952"
---
# <a name="mediainfo-resource-type"></a>mediaInfo 资源类型

命名空间：microsoft.graph

提示操作中使用的媒体信息。

## <a name="properties"></a>属性
| 属性       | 类型    | 说明                      |
|:---------------|:--------|:---------------------------------|
| resourceId     | String  | 可选。 用于唯一标识资源。 如果传入，提示 uri 将针对此 resourceId 缓存为密钥。 |
| uri            | String  | 将播放的提示的路径。 当前仅支持 Wave 文件 (.wav) 格式、单通道、16 位样本，采样率为 16，000 (16KHz) 采样率。 |


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

