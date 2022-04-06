---
title: imageInfo 资源类型
description: 表示活动对象的 visualInfo 部分中的属性的复杂类型。
ms.localizationpriority: medium
ms.prod: project-rome
doc_type: resourcePageType
author: ailae
ms.openlocfilehash: a123ea442fe4309ea96962b4155e0f36909fee7b
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723768"
---
# <a name="imageinfo-resource-type"></a>imageInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示活动对象的 [visualInfo](../resources/projectrome-visualinfo.md) 部分中的[属性的复杂类型](../resources/projectrome-activity.md)。

## <a name="properties"></a>属性

| 属性      | 类型    | 说明                                                                                                                                              |
| :------------ | :------ | :------------------------------------------------------------------------------------------------------------------------------------------------------- |
| iconUrl       | String  | 可选;指向表示用于生成活动的应用程序的图标的 URI                                                      |
| alternateText | String  | 可选;图像可选文字辅助内容                                                                                                      |
| addImageQuery | Boolean | 可选;参数，用于指示服务器能够动态呈现图像以响应参数化。 例如 - 高对比度图像 |

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

<!--
{
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
