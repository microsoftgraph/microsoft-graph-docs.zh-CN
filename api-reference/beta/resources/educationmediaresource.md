---
title: educationMediaResource 资源类型
description: 表示 educationAssignment 的媒体文件资源。 继承自 educationResource
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 54d7a6fa8d3b7fed03ed74ef2ceb5ab7e8bdc9c2
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220338"
---
# <a name="educationmediaresource-resource-type"></a>educationMediaResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [educationAssignment](educationassignment.md)的媒体文件资源。 继承自 [educationResource](educationresource.md)。

Upload这些文件提交到与分配或提交关联的 **fileResource** 目录。

以下文件类型是媒体资源：、 `webm` `mkv` 和 `avi` `wmv` `mp4` `m4v` `mpg` `mpeg` `m2v` `jpg` `png` `gif` `bmp` `heic` `jpeg` `psd` `mp3` `m4a` 。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|fileUrl|String|文件在共享点文件夹上的位置。 必需|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.educationMediaResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationMediaResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


