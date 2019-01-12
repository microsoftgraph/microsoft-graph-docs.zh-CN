---
title: imageInfo 资源类型
description: 代表活动对象的 visualInfo 部件中的**属性**属性的复杂类型。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: a17fe40f53308a0b1b1f587425d2afb019f84bb5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982363"
---
# <a name="imageinfo-resource-type"></a>imageInfo 资源类型

代表[活动](../resources/projectrome-activity.md)对象的[visualInfo](../resources/projectrome-visualinfo.md)部件中的**属性**属性的复杂类型。

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|iconUrl | 字符串 | 可选;指向一个表示用于生成活动的应用程序图标的 URI|
|alternateText | 字符串 | 可选;可选文字辅助内容的图像|
|addImageQuery | 布尔 | 可选;参数一起用来指示服务器是能够呈现动态以响应参数化的图像。 例如 – 高对比度图像|

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
