---
title: imageInfo 资源类型
description: 一个复杂类型，用于表示 activity 对象的 visualInfo 部分中**的属性属性**。
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: resourcePageType
ms.openlocfilehash: 35b4ad8573fe588c8e58123a36cc3acd97122fe2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447050"
---
# <a name="imageinfo-resource-type"></a>imageInfo 资源类型

命名空间： microsoft. graph

一个复杂类型，用于表示[activity](../resources/projectrome-activity.md)对象的[visualInfo](../resources/projectrome-visualinfo.md)部分中**的属性属性**。

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|iconUrl | String | Optional指向代表用于生成活动的应用程序的图标的 URI|
|alternateText | String | Optional图像的可选文本可访问内容|
|addImageQuery | 布尔 | Optional用于指示服务器能够动态呈现图像以响应参数化的参数。 例如-高对比度图像|

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
