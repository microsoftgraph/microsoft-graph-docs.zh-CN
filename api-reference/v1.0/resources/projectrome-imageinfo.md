---
title: imageInfo 资源类型
description: 表示活动对象的 visualInfo部分中的属性的复杂类型。
ms.localizationpriority: medium
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: cf76bd7e81f913f9641568bbd20c62a1c3ed16a8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019193"
---
# <a name="imageinfo-resource-type"></a>imageInfo 资源类型

命名空间：microsoft.graph

表示活动对象的[visualInfo](../resources/projectrome-visualinfo.md)部分中的[属性的复杂类型](../resources/projectrome-activity.md)。 

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|iconUrl | String | 可选;指向表示用于生成活动的应用程序的图标的 URI|
|alternateText | String | 可选;图像可选文字辅助内容|
|addImageQuery | 布尔值 | 可选;参数，用于指示服务器能够动态呈现图像以响应参数化。 例如 - 高对比度图像|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

